---
title: Overview Supported Fields
excerpt: >-
  Below you see 2 tables: supported fields for job sync and the supported fields
  for candidate sync for all the different supported ATS's.
deprecated: false
hidden: true
metadata:
  robots: index
---
<Embed typeOfEmbed="iframe" url="https://docs.google.com/spreadsheets/d/e/2PACX-1vTTdWlZtE6qfdXXUsiQb81ozfPVTm7LnjBTy1sQJLJhyabqDlFd_PjjPegi7rdC-v5UawKkJ0E4G09B/pubhtml?gid=1403645474&single=true&widget=true&headers=false" html="false" iframe="true" href="https://docs.google.com/spreadsheets/d/e/2PACX-1vTTdWlZtE6qfdXXUsiQb81ozfPVTm7LnjBTy1sQJLJhyabqDlFd_PjjPegi7rdC-v5UawKkJ0E4G09B/pubhtml?gid=1403645474&single=true&widget=true&headers=false" height="965px" width="1057px" />

<HTMLBlock>{`
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>Supported Fields Job Symc</title>
    <style>
        /* Container für die Tabelle */
        .table-container {
            width: 100%;
            overflow-x: auto;
            max-height: 750px; /* Optional: Höhe begrenzen */
        }

        /* Stil für die Tabelle */
        table {
            border-collapse: collapse;
            width: 100%;
        }

        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }

        th {
            background-color: #f2f2f2;
        }

        /* Fixierte erste Spalte */
        th:first-child, td:first-child {
            position: sticky;
            left: 0;
            background-color: #fff; /* Hintergrund für Sichtbarkeit */
            z-index: 1; /* Damit sie über anderen Zellen liegt */
            min-width: 150px; /* Optional: Breite der fixierten Spalte */
        }

        /* Scrollbar-Styling (optional) */
        .table-container::-webkit-scrollbar {
            height: 10px;
        }
        .table-container::-webkit-scrollbar-thumb {
            background: #888;
        }
    </style>
</head>
<body>
    <h2>Supported Fields Job Symc</h2>
    <div class="table-container">
        <table id="sheetTable">
            <thead>
                <tr id="headerRow"></tr>
            </thead>
            <tbody id="bodyRows"></tbody>
        </table>
    </div>

    <script>
        // URL für CSV-Export deiner Google Sheets
        const csvUrl = "https://docs.google.com/spreadsheets/d/e/2PACX-1vTTdWlZtE6qfdXXUsiQb81ozfPVTm7LnjBTy1sQJLJhyabqDlFd_PjjPegi7rdC-v5UawKkJ0E4G09B/pub?gid=1403645474&output=csv";

        // Daten abrufen und Tabelle füllen
        fetch(csvUrl)
            .then(response => response.text())
            .then(data => {
                // CSV in Zeilen aufteilen
                const rows = data.split('\n').map(row => row.split(','));

                // Header (erste Zeile) einfügen
                const headerRow = document.getElementById('headerRow');
                rows[0].forEach(cell => {
                    const th = document.createElement('th');
                    th.textContent = cell;
                    headerRow.appendChild(th);
                });

                // Datenzeilen einfügen
                const bodyRows = document.getElementById('bodyRows');
                for (let i = 1; i < rows.length; i++) {
                    if (rows[i].length > 1) { // Ignoriere leere Zeilen
                        const tr = document.createElement('tr');
                        rows[i].forEach(cell => {
                            const td = document.createElement('td');
                            td.textContent = cell;
                            tr.appendChild(td);
                        });
                        bodyRows.appendChild(tr);
                    }
                }
            })
            .catch(error => console.error('Fehler beim Laden der Daten:', error));
    </script>
</body>
</html>
`}</HTMLBlock>