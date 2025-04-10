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
            min-width:230px; /* Einheitliche feste Breite für alle Spalten */
            box-sizing: border-box; /* Padding wird in die Breite einbezogen */
        }
        th:first-child, td:first-child {
            position: sticky;
            left: 0;
            background-color: white;
            z-index: 3; /* Höherer z-index für die erste Spalte */
            min-width: 210px; /* Feste Breite für die erste Spalte */
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
            height: 30px;
            vertical-align: middle;
        
        }
        td.not-synced {
            font-size: 70%; /* ❌ bleibt 30% kleiner */
        }
        .large-logo {
            width: 400px;
            height: auto;
        }
        .recruitee-logo {
            width: 400px;
            height: auto;
        }
        .coveto-logo {
            width: 400px;
            height: auto;
        }
        .Hr4you-logo {
            width: 500px;
            height: auto;
        }
        .rexx-logo {
            width: 250px;
            height: auto;
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
                    <th style="min-width: 150px;"><img class="large-logo" src="https://www.guidecom.de/_assets/407aa76fe6bede19af48e7793075494f/img/logo_guidecom.svg" alt="GuideCom Logo"></th>
                    <th style="width: 150px;"><svg width="100" height="20" viewBox="0 0 122 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="" shape-rendering="geometricPrecision" data-testid="a:header::s:navigation-bar"><path d="M0 1.26011H0.486088C3.24829 1.26011 6.00999 1.25658 8.7722 1.26163C9.96555 1.26415 11.1187 1.46395 12.2135 1.97001C13.8281 2.71624 14.927 3.92362 15.4498 5.62243C15.9957 7.39642 15.9977 9.17596 15.2321 10.8889C14.2554 13.0736 12.4528 14.2325 10.1732 14.6316C9.10447 14.8188 7.99506 14.786 6.90275 14.8224C6.08741 14.8496 5.27056 14.8279 4.39942 14.8279V23.1196H0V1.26011ZM4.42707 10.8617C5.97179 10.8617 7.48937 10.901 9.00393 10.8455C9.8047 10.8162 10.5446 10.4868 11.09 9.86265C11.8878 8.95043 12.0245 7.89945 11.5656 6.79904C11.0946 5.67036 10.1576 5.14715 8.98333 5.08559C7.9644 5.03211 6.93995 5.07247 5.91851 5.07147C5.42689 5.07147 4.93527 5.07147 4.42707 5.07147V10.8611V10.8617Z" fill="currentColor"></path><path d="M32.6875 16.1452C30.6019 16.1452 28.5721 16.1452 26.5418 16.1452C24.5115 16.1452 22.5133 16.1452 20.5001 16.1452C20.4554 17.6447 21.5904 19.0564 23.1919 19.4772C25.1629 19.9954 26.8539 19.5277 28.2127 17.9726C28.2509 17.9288 28.2886 17.8833 28.3303 17.843C28.3504 17.8233 28.3795 17.8127 28.4484 17.7723C29.4467 18.4838 30.4621 19.2068 31.5097 19.953C30.5647 21.2229 29.4291 22.1977 28.0126 22.8269C22.7843 25.1488 16.908 21.8229 16.1937 16.1361C15.8418 13.3364 16.4812 10.8081 18.4034 8.7036C20.3342 6.59005 22.7898 5.80347 25.6068 6.0956C27.9317 6.33677 29.8433 7.34637 31.2141 9.26718C32.6835 11.3262 33.0585 13.6361 32.6875 16.1442V16.1452ZM28.743 13.0049C28.2624 10.8293 26.5805 9.61381 24.2782 9.72683C22.4746 9.81563 20.8268 11.2849 20.6283 13.0049H28.743Z" fill="currentColor"></path><path d="M113.14 23.5439C108.027 23.5404 104.363 19.8668 104.367 14.7461C104.37 9.76525 108.169 6.03311 113.228 6.04017C118.249 6.04723 122.007 9.86161 122 14.9459C121.993 19.8693 118.204 23.547 113.14 23.5439ZM113.126 19.6715C115.818 19.6791 117.843 17.6306 117.867 14.8753C117.892 12.0625 115.878 9.92065 113.196 9.90854C110.472 9.89592 108.467 11.9535 108.442 14.7845C108.418 17.5736 110.421 19.664 113.127 19.672L113.126 19.6715Z" fill="currentColor"></path><path d="M69.504 23.5439C64.4003 23.5384 60.687 19.8476 60.7051 14.7996C60.7237 9.73901 64.4677 6.03411 69.5578 6.04017C74.575 6.04622 78.2978 9.81469 78.2873 14.8773C78.2767 19.8754 74.5534 23.5495 69.5045 23.5439H69.504ZM69.4693 19.6715C72.228 19.6741 74.1894 17.673 74.1945 14.8531C74.1995 12.0357 72.1812 9.90803 69.5035 9.90853C66.8343 9.90853 64.8055 12.016 64.7979 14.7971C64.7899 17.6332 66.7413 19.6695 69.4693 19.672V19.6715Z" fill="currentColor"></path><path d="M94.5416 23.1869H90.4669V22.6087C90.4669 19.0522 90.4669 15.4961 90.4669 11.9396C90.4669 10.4083 90.1161 10.0581 88.5844 10.0581C87.6052 10.0581 86.626 10.0551 85.6468 10.0591C84.5509 10.0632 84.0995 10.5097 84.0985 11.6015C84.096 15.2751 84.0975 18.9487 84.0975 22.6218V23.1763H80.0047C80.0047 23.0003 80.0047 22.8438 80.0047 22.6869C80.0047 18.8377 80.0017 14.9885 80.0058 11.1394C80.0088 8.33255 82.1074 6.23616 84.9109 6.23212C86.4601 6.2301 88.0094 6.23111 89.5586 6.23212C92.4802 6.23313 94.5416 8.30178 94.5416 11.2332C94.5416 15.0385 94.5416 18.8438 94.5416 22.6486V23.1874V23.1869Z" fill="currentColor"></path><path d="M44.9082 18.0226H49.0402C49.4841 19.6558 50.211 20.2562 51.9095 20.2694C52.5982 20.2749 53.3074 20.1861 53.972 20.008C54.7381 19.8027 55.1136 19.1851 55.1105 18.4273C55.1075 17.6896 54.7793 17.1543 53.9976 16.9313C53.0626 16.6644 52.097 16.4999 51.1379 16.3263C49.8847 16.0993 48.6612 15.8066 47.5226 15.2007C44.8152 13.7602 44.8087 10.3939 46.1911 8.57092C47.2587 7.16222 48.7472 6.47352 50.4367 6.18391C52.5268 5.82517 54.5501 6.04768 56.4059 7.13094C57.9864 8.05326 58.8701 9.44328 58.9746 11.3409H54.9376C54.6415 9.74904 53.6714 9.34036 52.3172 9.30605C51.7411 9.29141 51.1484 9.3565 50.587 9.48718C49.8832 9.65116 49.4992 10.1491 49.4514 10.7723C49.3901 11.5694 49.6299 12.1396 50.3512 12.4004C51.1238 12.6795 51.9487 12.8333 52.7625 12.9741C54.2143 13.2254 55.673 13.4287 56.9931 14.1527C58.7871 15.1366 59.3928 16.7789 59.141 18.6624C58.8117 21.1256 57.2389 22.5141 54.9763 23.1569C52.4016 23.8885 49.8822 23.7129 47.5503 22.282C46.094 21.3884 45.2068 20.0736 44.9107 18.3768C44.8937 18.2784 44.9087 18.1745 44.9087 18.0226H44.9082Z" fill="currentColor"></path><path d="M44.0776 6.25128V10.0581C43.8333 10.0581 43.5906 10.0581 43.3478 10.0581C42.3686 10.0581 41.3893 10.0551 40.4101 10.0591C39.3062 10.0636 38.8413 10.5263 38.8403 11.6393C38.8362 15.313 38.8388 18.9861 38.8388 22.6597C38.8388 22.8186 38.8388 22.978 38.8388 23.1743H34.7807V22.7172C34.7807 18.8387 34.7756 14.9608 34.7822 11.0823C34.7867 8.31993 36.8718 6.2422 39.6365 6.23211C40.9812 6.22706 42.3258 6.2306 43.6705 6.23211C43.7987 6.23211 43.9263 6.24372 44.0776 6.25078V6.25128Z" fill="currentColor"></path><path d="M101.903 23.1871H97.7424V8.43262H101.903V23.1871Z" fill="currentColor"></path><path d="M99.8151 5.87619C98.2638 5.88275 97.0845 4.71321 97.0916 3.17535C97.0986 1.65969 98.3191 0.419508 99.802 0.421022C101.313 0.422536 102.555 1.66725 102.559 3.18443C102.563 4.69504 101.366 5.86963 99.8151 5.87619Z" fill="currentColor"></path></svg></th>
                    <th style="width: 150px;"><img src="https://www.cornerstoneondemand.com/_next/image/?url=https%3A%2F%2Fcdn.sanity.io%2Fimages%2F43ea2a5t%2Fcsod-new%2Fd81c21c51a9626f632933d779140d4638ae1f744-939x146.svg&w=384&q=75" alt="Cornerstone Logo"></th>
                    <th style="width: 150px;"><img src="https://www.workday.com/content/dam/web/zz/images/logos/workday/workday-logo.svg#icon" alt="Workday Logo"></th>
                    <th style="width: 150px;"><img src="https://go.zvoove.com/hubfs/zvoove-Logo_Cookies.png" alt="Zvoove Logo"></th>
                    <th style="width: 150px;"><img src="https://softgarden.com/wp-content/uploads/2023/06/logo_light.png" alt="Softgarden (XML) Logo">[XML]</th>
                    <th style="width: 150px;"><img src="https://softgarden.com/wp-content/uploads/2023/06/logo_light.png" alt="Softgarden (API) Logo">[API]</th>
                    <th style="width: 150px;"><img src="https://www.umantis.com/wp-content/uploads/2024/11/Abacus_Umantis_Logo_Farbe_Claim_klein.png" alt="Umantis Logo"></th>
                    <th style="width: 150px;"><img src="https://www.dvinci.de/wp-content/smush-webp/2020/10/brand_dvinci@2x.png.webp" alt="D.vinci Logo"></th>
                    <th style="width: 150px;"><img src="https://www.b-ite.de/images/logo-8b4a2b5bccdda5af4b02.svg" alt="B-ite Logo"></th>
                    <th style="width: 150px;"><img src="https://www.hrworks.de/wp-content/uploads/HR_WORKS_LOGO_RGB.svg" alt="HRworks Logo"></th>
                    <th style="width: 150px;"><img src="https://www.cegid.com/de/wp-content/uploads/sites/8/2023/04/cegid-logo-blue.svg" alt="Cegid Logo"></th>
                    <th style="width: 150px;"><svg class="logosvg" width="56" height="32" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M52.496 8.811h-3.054v8.364L43.664 9.32c-.224-.286-.578-.513-.977-.513l-4.26.005v16.722h4.894v-8.345l5.77 7.849c.221.293.587.479.99.479h2.415c1.016 0 1.84-.8 1.84-1.787V10.597c0-.987-.824-1.786-1.84-1.786ZM24.954 17.19c0-1.973-1.655-3.58-3.689-3.58-2.033 0-3.688 1.607-3.688 3.579 0 1.973 1.655 3.578 3.688 3.578 2.034 0 3.69-1.604 3.69-3.578Zm4.907-.007c0 4.603-3.846 8.334-8.592 8.334-4.744 0-8.59-3.731-8.59-8.334s3.846-8.335 8.591-8.335c4.745 0 8.59 3.731 8.59 8.335Zm1.222-13.735v2.962h4.895V1.66h-3.06c-1.017 0-1.835.8-1.835 1.788v-.001Zm0 22.069h4.895V8.828h-4.895v16.688ZM8.4 8.828h3.053v11.938c.002 5.246-4.382 9.5-9.79 9.5v-4.751c2.698 0 4.896-2.13 4.896-4.749V10.62c0-.987.823-1.792 1.84-1.792Z" fill="#000"></path></svg></th>
                    <th style="width: 150px;"><img src="https://kenjo-company-website.cdn.prismic.io/kenjo-company-website/b0934848-ddd6-4e63-ae91-a3ee3f3a4b5a_kenjo-horizontal-logo.svg?fit=max&w=384" alt="Kenjo Logo"></th>
                    <th style="width: 180px;"><img width="180px" src="https://www.erecruiter.net/wp-content/uploads/2020/04/Logo-eRecruiter-0219-RZ-Green.png" alt="eRecruiter Logo"></th>
                    <th style="width: 150px;"><img src="https://www.lever.co/wp-content/uploads/2022/09/Lever_Employ_Logo_Horizontal_Turquoise_Black.png" alt="Lever Logo"></th>
                    <th style="width: 150px;"><img src="https://upload.wikimedia.org/wikipedia/commons/c/c5/Factorial_company_logo_in_radical_red_color_with_text_saying_Factorial_in_Fira_font_type.png" alt="Factorial Logo"></th>
                    <th style="width: 150px;"><img src="https://images.teamtailor-cdn.com/images/s3/teamtailor-production/gallery_picture/image_uploads/2da198be-dbf8-4865-9e24-ea6dcaad606b/original.png" alt="TeamTailor Logo"></th>
                    <th style="width: 150px;"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6b/Greenhouse_logo.png/800px-Greenhouse_logo.png" alt="Greenhouse Logo"></th>
                    <th style="width: 150px;"><img src="https://hr-path.com/wp-content/uploads/2021/09/SAP_SuccessF_horz_R_pos_blugld.png" alt="Successfactors Logo"></th>
                    <th style="width: 150px;"><img class="recruitee-logo" src="https://www.one-click-recruiting.de/wp-content/uploads/2023/02/Recruitee-logo.png" alt="Recuitee Logo"></th>
                    <th style="width: 150px;"><img src="https://www.smartrecruiters.com/wp-content/themes/smartrecruiters/img/2024/SmartRecruiters-Logo.svg" alt="SmartRecruiters Logo"></th>
                    <th style="width: 150px;"><img class="hr4you-logo" src="https://www.hr4you.de/wp-content/uploads/2021/08/HR4YOU-neuesLogo_cmyk.png" alt="HR4You Logo"></th>
                    <th style="width: 150px;"><img class="coveto-logo" src="https://www.personalwirtschaft.de/wp-content/uploads/2022/11/coveto-b-g.png" alt="Coveto Logo"></th>
                    <th style="width: 150px;"><img src="https://www.heyrecruit.de/img/heyrecruit_logo_dark.svg" alt="Heyrecruit Logo"></th>
                    <th style="width: 150px;"><img class="rexx-logo" src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8e/Rexx-systems-logo.svg/2560px-Rexx-systems-logo.svg.png" alt="Rexx Logo"></th>
                </tr>
            </thead>
            <tbody>
                <tr><td>external_id</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>title</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>description</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>posting_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>application_url</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>❌</td><td>❌</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>status</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>remote</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>location_name</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>street</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>postcode</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>city</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>country</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>longitude</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>latitude</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>language</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>category</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>work_schedule</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>employment_type</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>start_date</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contract_limitation</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>senority</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>❌</td><td>✅</td><td>✅</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_name</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_email</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_title</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>contact_phone</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_from</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_to</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_currency</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>salary_frequency</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
                <tr><td>screening_questions</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td style="font-size: 70%;">❌</td><td>✅</td><td>✅</td><td style="font-size: 70%;">❌</td><td>✅</td><td style="font-size: 70%;">❌</td><td></td><td></td><td></td><td></td></tr>
        </table>
    </div>
</body>
</html>
`}</HTMLBlock>