---
layout: post
title:  "Metro times experiment"
date:   2025-04-13
excerpt: "Playing around to try get simple train times"
tag: [Life]
comments: false
---
I wanted to try pull live deaprture times for a specific station in a very quick experiment. See results below:


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>South Shields Metro Departures</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 20px;
        }
        h1 {
            color: #333;
        }
        .departures {
            margin-top: 20px;
        }
        .departure {
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <h1>South Shields Metro Departures</h1>
    <div id="departures" class="departures">Loading...</div>

    <script>
        async function fetchDepartures() {
            const stationCode = "SSS"; // South Shields station code
            const platformNumber = 2; // Adjust platform number as needed
            const apiUrl = `https://metro-rti.nexus.org.uk/api/times/${stationCode}/${platformNumber}`;
            
            try {
                const response = await fetch(apiUrl, {
                    headers: {
                        "User-Agent": "okhttp/3.12.1"
                    }
                });

                if (!response.ok) {
                    throw new Error(`Error fetching data: ${response.status}`);
                }

                const data = await response.json();
                displayDepartures(data);
            } catch (error) {
                document.getElementById("departures").innerText = `Failed to load data: ${error.message}`;
            }
        }

        function displayDepartures(data) {
            const departuresContainer = document.getElementById("departures");
            departuresContainer.innerHTML = ""; // Clear loading text

            if (data.length === 0) {
                departuresContainer.innerText = "No upcoming departures.";
                return;
            }

            data.forEach(departure => {
                const departureElement = document.createElement("div");
                departureElement.className = "departure";
                departureElement.innerText = `Train ${departure.trn}: Due in ${departure.dueIn} minutes`;
                departuresContainer.appendChild(departureElement);
            });
        }

        // Fetch departures on page load
        fetchDepartures();
    </script>
</body>
</html>
