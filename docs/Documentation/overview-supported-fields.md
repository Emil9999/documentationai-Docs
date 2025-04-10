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
<HTMLBlock>{`
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Integrationen Vergleich</title>
    <style>
        .table-container {
            width: 137.5%; /* Breite der Tabelle */
            overflow: auto; /* Scrollen in beide Richtungen */
            box-shadow: 0 6px 30px -2px rgba(0, 0, 0, 0.12);
            border-radius: 0.5rem;
            background-color: white;
            max-height: 80vh; /* Begrenzt die Höhe für vertikales Scrollen */
            position: relative;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            font-family: monospace;
            table-layout: fixed; /* Erzwingt feste Spaltenbreiten */
        }
        th, td {
            padding: 8px;
            text-align: center;
            border-bottom: 1px solid #e5e7eb;
            width: 250px; /* Einheitliche feste Breite für alle Spalten */
            box-sizing: border-box; /* Padding wird in die Breite einbezogen */
        }
        th:first-child, td:first-child {
            position: sticky;
            left: 0;
            background-color: white;
            z-index: 3; /* Höherer z-index für die erste Spalte */
            width: 300px; /* Feste Breite für die erste Spalte */
            text-align: left;
        }
        th {
            position: sticky;
            top: 0;
            background-color: #f9fafb;
            z-index: 2; /* Header über Zellen, unter erster Spalte */
        }
        th:first-child {
            z-index: 4; /* Field bleibt über allem */
            background-color: #f9fafb; /* Gleicher Hintergrund wie Header */
        }
        img {
            height: 20px;
            vertical-align: middle;
        }
        .not-synced {
            font-size: 70%; /* ❌ bleibt 30% kleiner */
        }
    </style>
</head>
<body>
    <div class="table-container">
        <table>
            <thead>
                <tr>
                    <th>Field</th>
                    <th><img src="https://www.new-work.se/static/onlyfy-logo.png" alt="Onlyfy Logo"></th>
                    <th><img src="https://www.guidecom.de/wp-content/uploads/guidecom-logo.png" alt="GuideCom Logo"></th>
                    <th><img src="https://www.personio.com/wp-content/uploads/personio-logo.svg" alt="Personio Logo"></th>
                    <th><img src="https://www.cornerstoneondemand.com/wp-content/uploads/cornerstone-logo.png" alt="Cornerstone Logo"></th>
                    <th><img src="https://www.workday.com/content/dam/web/en-us/images/workday-logo.svg" alt="Workday Logo"></th>
                    <th><img src="https://www.zvoove.com/wp-content/uploads/zvoove-logo.png" alt="Zvoove Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (XML) Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (API) Logo"></th>
                    <th><img src="https://www.umantis.com/wp-content/uploads/umantis-logo.png" alt="Umantis Logo"></th>
                    <th><img src="https://www.dvinci.de/wp-content/uploads/dvinci-logo.svg" alt="D.vinci Logo"></th>
                    <th>[Logo B-ite]</th>
                    <th><img src="https://www.hrworks.de/wp-content/uploads/hrworks-logo.png" alt="HRworks Logo"></th>
                    <th><img src="https://www.cegid.com/wp-content/uploads/cegid-logo.svg" alt="Cegid Logo"></th>
                    <th><img src="https://www.join.com/wp-content/uploads/join-logo.png" alt="Join Logo"></th>
                    <th><img src="https://www.kenjo.io/wp-content/uploads/kenjo-logo.svg" alt="Kenjo Logo"></th>
                    <th><img src="https://www.erecruiter.pl/wp-content/uploads/erecruiter-logo.png" alt="eRecruiter Logo"></th>
                    <th><img src="https://www.lever.co/wp-content/uploads/lever-logo.svg" alt="Lever Logo"></th>
                    <th><img src="https://www.factorialhr.com/wp-content/uploads/factorial-logo.png" alt="Factorial Logo"></th>
                    <th><img src="https://www.teamtailor.com/wp-content/uploads/teamtailor-logo.svg" alt="TeamTailor Logo"></th>
                    <th><img src="https://www.greenhouse.io/wp-content/uploads/greenhouse-logo.png" alt="Greenhouse Logo"></th>
                    <th><img src="https://www.sap.com/dam/application/shared/logos/successfactors-logo.svg" alt="Successfactors Logo"></th>
                    <th><img src="https://www.recruitmentsoftware.recruitee.com/wp-content/uploads/recruitee-logo.png" alt="Recuitee Logo"></th>
                    <th><img src="https://www.smartrecruiters.com/wp-content/uploads/smartrecruiters-logo.svg" alt="SmartRecruiters Logo"></th>
                    <th><img src="https://www.hr4you.de/wp-content/uploads/hr4you-logo.png" alt="HR4You Logo"></th>
                    <th>[Logo Coveto]</th>
                    <th><img src="https://www.heyrecruit.de/wp-content/uploads/heyrecruit-logo.png" alt="Heyrecruit Logo"></th>
                    <th><img src="https://www.rexx-systems.com/wp-content/uploads/rexx-logo.svg" alt="Rexx Logo"></th>
                </tr>
            </thead>
            <tbody>
                            <tr><td>external_id</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>title</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>description</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>posting_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>application_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>status</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>remote</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>location_name</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>street</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>postcode</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>city</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>country</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>longitude</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>latitude</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>language</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>category</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>work_schedule</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>employment_type</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>start_date</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contract_limitation</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>senority</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_name</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_email</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_title</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_phone</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_from</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_to</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_currency</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_frequency</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>screening_questions</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>❌</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td>❌</td><td>✅</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
            </tbody>
        </table>
    </div>
</body>
</html>
`}</HTMLBlock>

<HTMLBlock>{`
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Integrationen Vergleich</title>
    <style>
        .table-container {
            width: 137,5%;
            overflow-x: auto;
            box-shadow: 0 6px 30px -2px rgba(0, 0, 0, 0.12);
            border-radius: 0.5rem;
            background-color: white;
            max-height: 80vh; /* Begrenzt die Höhe, damit Scrollen möglich ist */
            position: relative;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            font-family: monospace;
        }
        th, td {
            padding: 8px;
            text-align: center;
            border-bottom: 1px solid #e5e7eb;
            width: 130px; /* Feste Spaltenbreite */
        }
        th:first-child, td:first-child {
            position: sticky;
            left: 0;
            background-color: white;
            z-index: 2; /* Höherer z-index für die erste Spalte */
            min-width: 150px; /* Erste Spalte bleibt bei 150px */
            text-align: left;
        }
        th {
            position: sticky;
            top: 0;
            background-color: #f9fafb;
            z-index: 1; /* Header bleibt über den Zellen, aber unter der ersten Spalte */
        }
        img {
            height: 20px;
            vertical-align: middle;
        }
        .not-synced {
            font-size: 70%; /* ❌ wird 30% kleiner */
        }
    </style>
</head>
<body>
    <div class="table-container">
        <table>
            <thead>
                <tr>
                    <th>Field</th>
                    <th><img src="https://www.new-work.se/static/onlyfy-logo.png" alt="Onlyfy Logo"></th>
                    <th><img src="https://www.guidecom.de/wp-content/uploads/guidecom-logo.png" alt="GuideCom Logo"></th>
                    <th><img src="https://www.personio.com/wp-content/uploads/personio-logo.svg" alt="Personio Logo"></th>
                    <th><img src="https://www.cornerstoneondemand.com/wp-content/uploads/cornerstone-logo.png" alt="Cornerstone Logo"></th>
                    <th><img src="https://www.workday.com/content/dam/web/en-us/images/workday-logo.svg" alt="Workday Logo"></th>
                    <th><img src="https://www.zvoove.com/wp-content/uploads/zvoove-logo.png" alt="Zvoove Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (XML) Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (API) Logo"></th>
                    <th><img src="https://www.umantis.com/wp-content/uploads/umantis-logo.png" alt="Umantis Logo"></th>
                    <th><img src="https://www.dvinci.de/wp-content/uploads/dvinci-logo.svg" alt="D.vinci Logo"></th>
                    <th>[Logo B-ite]</th>
                    <th><img src="https://www.hrworks.de/wp-content/uploads/hrworks-logo.png" alt="HRworks Logo"></th>
                    <th><img src="https://www.cegid.com/wp-content/uploads/cegid-logo.svg" alt="Cegid Logo"></th>
                    <th><img src="https://www.join.com/wp-content/uploads/join-logo.png" alt="Join Logo"></th>
                    <th><img src="https://www.kenjo.io/wp-content/uploads/kenjo-logo.svg" alt="Kenjo Logo"></th>
                    <th><img src="https://www.erecruiter.pl/wp-content/uploads/erecruiter-logo.png" alt="eRecruiter Logo"></th>
                    <th><img src="https://www.lever.co/wp-content/uploads/lever-logo.svg" alt="Lever Logo"></th>
                    <th><img src="https://www.factorialhr.com/wp-content/uploads/factorial-logo.png" alt="Factorial Logo"></th>
                    <th><img src="https://www.teamtailor.com/wp-content/uploads/teamtailor-logo.svg" alt="TeamTailor Logo"></th>
                    <th><img src="https://www.greenhouse.io/wp-content/uploads/greenhouse-logo.png" alt="Greenhouse Logo"></th>
                    <th><img src="https://www.sap.com/dam/application/shared/logos/successfactors-logo.svg" alt="Successfactors Logo"></th>
                    <th><img src="https://www.recruitmentsoftware.recruitee.com/wp-content/uploads/recruitee-logo.png" alt="Recuitee Logo"></th>
                    <th><img src="https://www.smartrecruiters.com/wp-content/uploads/smartrecruiters-logo.svg" alt="SmartRecruiters Logo"></th>
                    <th><img src="https://www.hr4you.de/wp-content/uploads/hr4you-logo.png" alt="HR4You Logo"></th>
                    <th>[Logo Coveto]</th>
                    <th><img src="https://www.heyrecruit.de/wp-content/uploads/heyrecruit-logo.png" alt="Heyrecruit Logo"></th>
                    <th><img src="https://www.rexx-systems.com/wp-content/uploads/rexx-logo.svg" alt="Rexx Logo"></th>
                </tr>
            </thead>
            <tbody>
                <tr><td>external_id</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>title</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>description</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>posting_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>application_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>status</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>remote</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>location_name</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>street</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>postcode</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>city</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>country</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>longitude</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>latitude</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>language</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>category</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>work_schedule</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>employment_type</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>start_date</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contract_limitation</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>senority</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_name</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_email</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_title</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_phone</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_from</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_to</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_currency</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_frequency</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>screening_questions</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
            </tbody>
        </table>
    </div>
</body>
</html>
`}</HTMLBlock>

<HTMLBlock>{`
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Integrationen Vergleich</title>
    <style>
        .table-container {
            width: 137.5%; /* Zurück auf 137.5% */
            overflow: auto; /* Scrollen in beide Richtungen */
            box-shadow: 0 6px 30px -2px rgba(0, 0, 0, 0.12);
            border-radius: 0.5rem;
            background-color: white;
            max-height: 80vh; /* Begrenzt die Höhe für vertikales Scrollen */
            position: relative;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            font-family: monospace;
        }
        th, td {
            padding: 8px;
            text-align: center;
            border-bottom: 1px solid #e5e7eb;
            width: 250px; /* Fixe, breitere Spaltenbreite für alle Systeme */
        }
        th:first-child, td:first-child {
            position: sticky;
            left: 0;
            background-color: white;
            z-index: 3; /* Höherer z-index für die erste Spalte */
            width: 300px; /* Breiter, um Überlappungen zu vermeiden */
            text-align: left;
        }
        th {
            position: sticky;
            top: 0;
            background-color: #f9fafb;
            z-index: 2; /* Header über Zellen, unter erster Spalte */
        }
        th:first-child {
            z-index: 4; /* Field bleibt über allem */
            background-color: #f9fafb; /* Gleicher Hintergrund wie Header */
        }
        img {
            height: 20px;
            vertical-align: middle;
        }
        .not-synced {
            font-size: 70%; /* ❌ bleibt 30% kleiner */
        }
    </style>
</head>
<body>
    <div class="table-container">
        <table>
            <thead>
                <tr>
                    <th>Field</th>
                    <th><img src="https://www.new-work.se/static/onlyfy-logo.png" alt="Onlyfy Logo"></th>
                    <th><img src="https://www.guidecom.de/wp-content/uploads/guidecom-logo.png" alt="GuideCom Logo"></th>
                    <th><img src="https://www.personio.com/wp-content/uploads/personio-logo.svg" alt="Personio Logo"></th>
                    <th><img src="https://www.cornerstoneondemand.com/wp-content/uploads/cornerstone-logo.png" alt="Cornerstone Logo"></th>
                    <th><img src="https://www.workday.com/content/dam/web/en-us/images/workday-logo.svg" alt="Workday Logo"></th>
                    <th><img src="https://www.zvoove.com/wp-content/uploads/zvoove-logo.png" alt="Zvoove Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (XML) Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (API) Logo"></th>
                    <th><img src="https://www.umantis.com/wp-content/uploads/umantis-logo.png" alt="Umantis Logo"></th>
                    <th><img src="https://www.dvinci.de/wp-content/uploads/dvinci-logo.svg" alt="D.vinci Logo"></th>
                    <th>[Logo B-ite]</th>
                    <th><img src="https://www.hrworks.de/wp-content/uploads/hrworks-logo.png" alt="HRworks Logo"></th>
                    <th><img src="https://www.cegid.com/wp-content/uploads/cegid-logo.svg" alt="Cegid Logo"></th>
                    <th><img src="https://www.join.com/wp-content/uploads/join-logo.png" alt="Join Logo"></th>
                    <th><img src="https://www.kenjo.io/wp-content/uploads/kenjo-logo.svg" alt="Kenjo Logo"></th>
                    <th><img src="https://www.erecruiter.pl/wp-content/uploads/erecruiter-logo.png" alt="eRecruiter Logo"></th>
                    <th><img src="https://www.lever.co/wp-content/uploads/lever-logo.svg" alt="Lever Logo"></th>
                    <th><img src="https://www.factorialhr.com/wp-content/uploads/factorial-logo.png" alt="Factorial Logo"></th>
                    <th><img src="https://www.teamtailor.com/wp-content/uploads/teamtailor-logo.svg" alt="TeamTailor Logo"></th>
                    <th><img src="https://www.greenhouse.io/wp-content/uploads/greenhouse-logo.png" alt="Greenhouse Logo"></th>
                    <th><img src="https://www.sap.com/dam/application/shared/logos/successfactors-logo.svg" alt="Successfactors Logo"></th>
                    <th><img src="https://www.recruitmentsoftware.recruitee.com/wp-content/uploads/recruitee-logo.png" alt="Recuitee Logo"></th>
                    <th><img src="https://www.smartrecruiters.com/wp-content/uploads/smartrecruiters-logo.svg" alt="SmartRecruiters Logo"></th>
                    <th><img src="https://www.hr4you.de/wp-content/uploads/hr4you-logo.png" alt="HR4You Logo"></th>
                    <th>[Logo Coveto]</th>
                    <th><img src="https://www.heyrecruit.de/wp-content/uploads/heyrecruit-logo.png" alt="Heyrecruit Logo"></th>
                    <th><img src="https://www.rexx-systems.com/wp-content/uploads/rexx-logo.svg" alt="Rexx Logo"></th>
                </tr>
            </thead>
            <tbody>
                <tr><td>external_id</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>title</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>description</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>posting_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>application_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>status</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>remote</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>location_name</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>street</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>postcode</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>city</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>country</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>longitude</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>latitude</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>language</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>category</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>work_schedule</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>employment_type</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>start_date</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contract_limitation</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>senority</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_name</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_email</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_title</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_phone</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_from</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_to</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_currency</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_frequency</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>screening_questions</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
            </tbody>
        </table>
    </div>
</body>
</html>
`}</HTMLBlock>

<HTMLBlock>{`
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Fixierte Spalte Tabelle</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background-color: #f5f5f5;
    }

    .table-wrapper {
      width: 100%;
      overflow-x: auto;
    }

    table {
      width: 137%; /* Beibehaltung deiner Breite für Darstellung */
      border-collapse: collapse;
      min-width: 100%;
    }

    th, td {
      padding: 12px 16px;
      text-align: left;
      border: 1px solid #ddd;
      background-color: white;
      white-space: nowrap;
    }

    th {
      background-color: #f0f0f0;
      font-weight: bold;
    }

    /* Fixierte erste Spalte */
    td:first-child,
    th:first-child {
      position: sticky;
      left: 0;
      background-color: #ffffff;
      z-index: 2;
      box-shadow: 2px 0 5px rgba(0,0,0,0.1);
    }

    /* Optional: Header oben fixieren (nicht aktiv, falls gewünscht, kann ergänzt werden)
    thead th {
      position: sticky;
      top: 0;
      z-index: 3;
    }
    */

    /* Scrollbar Styling (optional) */
    .table-wrapper::-webkit-scrollbar {
      height: 10px;
    }
    .table-wrapper::-webkit-scrollbar-thumb {
      background-color: #ccc;
      border-radius: 10px;
    }
    .table-wrapper::-webkit-scrollbar-track {
      background-color: transparent;
    }

    @media (max-width: 768px) {
      th, td {
        padding: 10px 12px;
        font-size: 14px;
      }
    }
      }
    </style>
</head>
<body>
    <div class="table-container">
        <table>
            <thead>
                <tr>
                    <th>Field</th>
                    <th><img src="https://www.new-work.se/static/onlyfy-logo.png" alt="Onlyfy Logo"></th>
                    <th><img src="https://www.guidecom.de/wp-content/uploads/guidecom-logo.png" alt="GuideCom Logo"></th>
                    <th><img src="https://www.personio.com/wp-content/uploads/personio-logo.svg" alt="Personio Logo"></th>
                    <th><img src="https://www.cornerstoneondemand.com/wp-content/uploads/cornerstone-logo.png" alt="Cornerstone Logo"></th>
                    <th><img src="https://www.workday.com/content/dam/web/en-us/images/workday-logo.svg" alt="Workday Logo"></th>
                    <th><img src="https://www.zvoove.com/wp-content/uploads/zvoove-logo.png" alt="Zvoove Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (XML) Logo"></th>
                    <th><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (API) Logo"></th>
                    <th><img src="https://www.umantis.com/wp-content/uploads/umantis-logo.png" alt="Umantis Logo"></th>
                    <th><img src="https://www.dvinci.de/wp-content/uploads/dvinci-logo.svg" alt="D.vinci Logo"></th>
                    <th>[Logo B-ite]</th>
                    <th><img src="https://www.hrworks.de/wp-content/uploads/hrworks-logo.png" alt="HRworks Logo"></th>
                    <th><img src="https://www.cegid.com/wp-content/uploads/cegid-logo.svg" alt="Cegid Logo"></th>
                    <th><img src="https://www.join.com/wp-content/uploads/join-logo.png" alt="Join Logo"></th>
                    <th><img src="https://www.kenjo.io/wp-content/uploads/kenjo-logo.svg" alt="Kenjo Logo"></th>
                    <th><img src="https://www.erecruiter.pl/wp-content/uploads/erecruiter-logo.png" alt="eRecruiter Logo"></th>
                    <th><img src="https://www.lever.co/wp-content/uploads/lever-logo.svg" alt="Lever Logo"></th>
                    <th><img src="https://www.factorialhr.com/wp-content/uploads/factorial-logo.png" alt="Factorial Logo"></th>
                    <th><img src="https://www.teamtailor.com/wp-content/uploads/teamtailor-logo.svg" alt="TeamTailor Logo"></th>
                    <th><img src="https://www.greenhouse.io/wp-content/uploads/greenhouse-logo.png" alt="Greenhouse Logo"></th>
                    <th><img src="https://www.sap.com/dam/application/shared/logos/successfactors-logo.svg" alt="Successfactors Logo"></th>
                    <th><img src="https://www.recruitmentsoftware.recruitee.com/wp-content/uploads/recruitee-logo.png" alt="Recuitee Logo"></th>
                    <th><img src="https://www.smartrecruiters.com/wp-content/uploads/smartrecruiters-logo.svg" alt="SmartRecruiters Logo"></th>
                    <th><img src="https://www.hr4you.de/wp-content/uploads/hr4you-logo.png" alt="HR4You Logo"></th>
                    <th>[Logo Coveto]</th>
                    <th><img src="https://www.heyrecruit.de/wp-content/uploads/heyrecruit-logo.png" alt="Heyrecruit Logo"></th>
                    <th><img src="https://www.rexx-systems.com/wp-content/uploads/rexx-logo.svg" alt="Rexx Logo"></th>
                </tr>
            </thead>
            <tbody>
                <tr><td>external_id</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>title</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>description</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>posting_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>application_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>status</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>remote</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>location_name</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>street</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>postcode</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>city</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>country</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>longitude</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>latitude</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>language</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>category</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>work_schedule</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>employment_type</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>start_date</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contract_limitation</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>senority</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_name</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_email</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_title</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_phone</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_from</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_to</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_currency</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_frequency</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>screening_questions</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td class="not-synced">❌</td><td>✅</td><td>✅</td><td class="not-synced">❌</td><td>✅</td><td class="not-synced">❌</td><td></td><td></td><td></td><td></td></tr>
            </tbody>
        </table>
    </div>
</body>
</html>
`}</HTMLBlock>