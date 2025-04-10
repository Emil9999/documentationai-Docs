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
            min-width:150px; /* Einheitliche feste Breite für alle Spalten */
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
            height: 25px;
            vertical-align: middle;
        }
        .not-synced {
            font-size:50%; /* ❌ bleibt 30% kleiner */
        }
    </style>
</head>
<body>
    <div class="table-container">
        <table>
            <thead>
                <tr>
                    <th style="width: 150px;">Field</th>
                    <th style="width: 150px;"><img src="https://onlyfy.com/wp-content/themes/onlyfy/assets/icons/logo.svg" alt="Onlyfy Logo"></th>
                    <th style="width: 150px;"><img src="https://www.guidecom.de/_assets/407aa76fe6bede19af48e7793075494f/img/logo_guidecom.svg" alt="GuideCom Logo"></th>
                    <th style="width: 150px;"><img src="https://upload.wikimedia.org/wikipedia/commons/a/ab/Personio_logo_%282024%29.svg" alt="Personio Logo"></th>
                    <th style="width: 150px;"><img src="https://www.cornerstoneondemand.com/_next/image/?url=https%3A%2F%2Fcdn.sanity.io%2Fimages%2F43ea2a5t%2Fcsod-new%2Fd81c21c51a9626f632933d779140d4638ae1f744-939x146.svg&w=384&q=75" alt="Cornerstone Logo"></th>
                    <th style="width: 150px;"><img src="https://www.workday.com/content/dam/web/zz/images/logos/workday/workday-logo.svg#icon" alt="Workday Logo"></th>
                    <th style="width: 150px;"><img src="https://go.zvoove.com/hubfs/zvoove-Logo_Cookies.png" alt="Zvoove Logo"></th>
                    <th style="width: 150px;"><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (XML) Logo">[XML]</th>
                    <th style="width: 150px;"><img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (API) Logo">[API]</th>
                    <th style="width: 150px;"><img src="https://www.umantis.com/wp-content/uploads/2024/11/Abacus_Umantis_Logo_Farbe_Claim_klein.png" alt="Umantis Logo"></th>
                    <th style="width: 150px;"><img src="https://www.dvinci.de/wp-content/smush-webp/2020/10/brand_dvinci@2x.png.webp" alt="D.vinci Logo"></th>
                    <th style="width: 150px;"><img src="https://www.b-ite.de/images/logo-8b4a2b5bccdda5af4b02.svg" alt="B-ite Logo"></th>
                    <th style="width: 150px;"><img src="https://www.hrworks.de/wp-content/uploads/HR_WORKS_LOGO_RGB.svg" alt="HRworks Logo"></th>
                    <th style="width: 150px;"><img src="https://www.cegid.com/de/wp-content/uploads/sites/8/2023/04/cegid-logo-blue.svg" alt="Cegid Logo"></th>
                    <th style="width: 150px;"><svg class="logosvg" width="56" height="32" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M52.496 8.811h-3.054v8.364L43.664 9.32c-.224-.286-.578-.513-.977-.513l-4.26.005v16.722h4.894v-8.345l5.77 7.849c.221.293.587.479.99.479h2.415c1.016 0 1.84-.8 1.84-1.787V10.597c0-.987-.824-1.786-1.84-1.786ZM24.954 17.19c0-1.973-1.655-3.58-3.689-3.58-2.033 0-3.688 1.607-3.688 3.579 0 1.973 1.655 3.578 3.688 3.578 2.034 0 3.69-1.604 3.69-3.578Zm4.907-.007c0 4.603-3.846 8.334-8.592 8.334-4.744 0-8.59-3.731-8.59-8.334s3.846-8.335 8.591-8.335c4.745 0 8.59 3.731 8.59 8.335Zm1.222-13.735v2.962h4.895V1.66h-3.06c-1.017 0-1.835.8-1.835 1.788v-.001Zm0 22.069h4.895V8.828h-4.895v16.688ZM8.4 8.828h3.053v11.938c.002 5.246-4.382 9.5-9.79 9.5v-4.751c2.698 0 4.896-2.13 4.896-4.749V10.62c0-.987.823-1.792 1.84-1.792Z" fill="#000"></path></svg></th>
                    <th style="width: 150px;"><img src="https://www.kenjo.io/wp-content/uploads/kenjo-logo.svg" alt="Kenjo Logo"></th>
                    <th style="width: 150px;"><img src="https://www.erecruiter.pl/wp-content/uploads/erecruiter-logo.png" alt="eRecruiter Logo"></th>
                    <th style="width: 150px;"><img src="https://www.lever.co/wp-content/uploads/lever-logo.svg" alt="Lever Logo"></th>
                    <th style="width: 150px;"><img src="https://www.factorialhr.com/wp-content/uploads/factorial-logo.png" alt="Factorial Logo"></th>
                    <th style="width: 150px;"><img src="https://www.teamtailor.com/wp-content/uploads/teamtailor-logo.svg" alt="TeamTailor Logo"></th>
                    <th style="width: 150px;"><img src="https://www.greenhouse.io/wp-content/uploads/greenhouse-logo.png" alt="Greenhouse Logo"></th>
                    <th style="width: 150px;"><img src="https://www.sap.com/dam/application/shared/logos/successfactors-logo.svg" alt="Successfactors Logo"></th>
                    <th style="width: 150px;"><img src="https://www.recruitmentsoftware.recruitee.com/wp-content/uploads/recruitee-logo.png" alt="Recuitee Logo"></th>
                    <th style="width: 150px;"><img src="https://www.smartrecruiters.com/wp-content/uploads/smartrecruiters-logo.svg" alt="SmartRecruiters Logo"></th>
                    <th style="width: 150px;"><img src="https://www.hr4you.de/wp-content/uploads/hr4you-logo.png" alt="HR4You Logo"></th>
                    <th style="width: 150px;">[Logo Coveto]</th>
                    <th style="width: 150px;"><img src="https://www.heyrecruit.de/wp-content/uploads/heyrecruit-logo.png" alt="Heyrecruit Logo"></th>
                    <th style="width: 150px;"><img src="https://www.rexx-systems.com/wp-content/uploads/rexx-logo.svg" alt="Rexx Logo"></th>
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