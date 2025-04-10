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
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <meta http-equiv="Content-Style-Type" content="text/css">
  <title></title>
  <meta name="Generator" content="Cocoa HTML Writer">
  <meta name="CocoaVersion" content="2575.4">
  <style type="text/css">
    p.p1 {margin: 0.0px 0.0px 0.0px 0.0px; font: 12.0px Helvetica}
    .table-container {
        width: 100%; /* Adjusted to fit within the viewport */
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
<p class="p1">&lt;!DOCTYPE html&gt;</p>
<p class="p1">&lt;html lang="de"&gt;</p>
<p class="p1">&lt;head&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;meta charset="UTF-8"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;title&gt;Integrationen Vergleich&lt;/title&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;style&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>.table-container {</p>
<p class="p1"><span class="Apple-converted-space">            </span>width: 100%; /* Adjusted to fit within the viewport */</p>
<p class="p1"><span class="Apple-converted-space">            </span>overflow: auto; /* Scrollen in beide Richtungen */</p>
<p class="p1"><span class="Apple-converted-space">            </span>box-shadow: 0 6px 30px -2px rgba(0, 0, 0, 0.12);</p>
<p class="p1"><span class="Apple-converted-space">            </span>border-radius: 0.5rem;</p>
<p class="p1"><span class="Apple-converted-space">            </span>background-color: white;</p>
<p class="p1"><span class="Apple-converted-space">            </span>max-height: 80vh; /* Begrenzt die Höhe für vertikales Scrollen */</p>
<p class="p1"><span class="Apple-converted-space">            </span>position: relative;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>table {</p>
<p class="p1"><span class="Apple-converted-space">            </span>width: 100%;</p>
<p class="p1"><span class="Apple-converted-space">            </span>border-collapse: collapse;</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-family: monospace;</p>
<p class="p1"><span class="Apple-converted-space">            </span>table-layout: fixed; /* Erzwingt feste Spaltenbreiten */</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>th, td {</p>
<p class="p1"><span class="Apple-converted-space">            </span>padding: 8px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>text-align: center;</p>
<p class="p1"><span class="Apple-converted-space">            </span>border-bottom: 1px solid #e5e7eb;</p>
<p class="p1"><span class="Apple-converted-space">            </span>width: 250px; /* Einheitliche feste Breite für alle Spalten */</p>
<p class="p1"><span class="Apple-converted-space">            </span>box-sizing: border-box; /* Padding wird in die Breite einbezogen */</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>th:first-child, td:first-child {</p>
<p class="p1"><span class="Apple-converted-space">            </span>position: sticky;</p>
<p class="p1"><span class="Apple-converted-space">            </span>left: 0;</p>
<p class="p1"><span class="Apple-converted-space">            </span>background-color: white;</p>
<p class="p1"><span class="Apple-converted-space">            </span>z-index: 3; /* Höherer z-index für die erste Spalte */</p>
<p class="p1"><span class="Apple-converted-space">            </span>width: 300px; /* Feste Breite für die erste Spalte */</p>
<p class="p1"><span class="Apple-converted-space">            </span>text-align: left;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>th {</p>
<p class="p1"><span class="Apple-converted-space">            </span>position: sticky;</p>
<p class="p1"><span class="Apple-converted-space">            </span>top: 0;</p>
<p class="p1"><span class="Apple-converted-space">            </span>background-color: #f9fafb;</p>
<p class="p1"><span class="Apple-converted-space">            </span>z-index: 2; /* Header über Zellen, unter erster Spalte */</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>th:first-child {</p>
<p class="p1"><span class="Apple-converted-space">            </span>z-index: 4; /* Field bleibt über allem */</p>
<p class="p1"><span class="Apple-converted-space">            </span>background-color: #f9fafb; /* Gleicher Hintergrund wie Header */</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>img {</p>
<p class="p1"><span class="Apple-converted-space">            </span>height: 20px;</p>
<p class="p1"><span class="Apple-converted-space">            </span>vertical-align: middle;</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">        </span>.not-synced {</p>
<p class="p1"><span class="Apple-converted-space">            </span>font-size: 70%; /* ❌ bleibt 30% kleiner */</p>
<p class="p1"><span class="Apple-converted-space">        </span>}</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/style&gt;</p>
<p class="p1">&lt;/head&gt;</p>
<p class="p1">&lt;body&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div class="table-container"&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;table&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;thead&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;Field&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.new-work.se/static/onlyfy-logo.png" alt="Onlyfy Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.guidecom.de/wp-content/uploads/guidecom-logo.png" alt="GuideCom Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.personio.com/wp-content/uploads/personio-logo.svg" alt="Personio Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.cornerstoneondemand.com/wp-content/uploads/cornerstone-logo.png" alt="Cornerstone Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.workday.com/content/dam/web/en-us/images/workday-logo.svg" alt="Workday Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.zvoove.com/wp-content/uploads/zvoove-logo.png" alt="Zvoove Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (XML) Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.softgarden.com/wp-content/uploads/softgarden-logo.svg" alt="Softgarden (API) Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.umantis.com/wp-content/uploads/umantis-logo.png" alt="Umantis Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.dvinci.de/wp-content/uploads/dvinci-logo.svg" alt="D.vinci Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;[Logo B-ite]&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.hrworks.de/wp-content/uploads/hrworks-logo.png" alt="HRworks Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.cegid.com/wp-content/uploads/cegid-logo.svg" alt="Cegid Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.join.com/wp-content/uploads/join-logo.png" alt="Join Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.kenjo.io/wp-content/uploads/kenjo-logo.svg" alt="Kenjo Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.erecruiter.pl/wp-content/uploads/erecruiter-logo.png" alt="eRecruiter Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.lever.co/wp-content/uploads/lever-logo.svg" alt="Lever Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.factorialhr.com/wp-content/uploads/factorial-logo.png" alt="Factorial Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.teamtailor.com/wp-content/uploads/teamtailor-logo.svg" alt="TeamTailor Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.greenhouse.io/wp-content/uploads/greenhouse-logo.png" alt="Greenhouse Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.sap.com/dam/application/shared/logos/successfactors-logo.svg" alt="Successfactors Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.recruitmentsoftware.recruitee.com/wp-content/uploads/recruitee-logo.png" alt="Recuitee Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.smartrecruiters.com/wp-content/uploads/smartrecruiters-logo.svg" alt="SmartRecruiters Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.hr4you.de/wp-content/uploads/hr4you-logo.png" alt="HR4You Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;[Logo Coveto]&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.heyrecruit.de/wp-content/uploads/heyrecruit-logo.png" alt="Heyrecruit Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                    </span>&lt;th&gt;&lt;img src="https://www.rexx-systems.com/wp-content/uploads/rexx-logo.svg" alt="Rexx Logo"&gt;&lt;/th&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/thead&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;tbody&gt;</p>
<p class="p1"><span class="Apple-converted-space">                            </span>&lt;tr&gt;&lt;td&gt;external_id&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;title&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;description&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;posting_url&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;application_url&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;status&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;remote&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;location_name&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;street&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;postcode&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;city&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;country&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;longitude&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;latitude&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;language&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;category&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;work_schedule&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;employment_type&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;start_date&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;contract_limitation&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;senority&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;contact_name&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;contact_email&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;contact_title&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;contact_phone&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;salary&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;salary_from&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;salary_to&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;salary_currency&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;salary_frequency&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">                </span>&lt;tr&gt;&lt;td&gt;screening_questions&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;✅&lt;/td&gt;&lt;td&gt;❌&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;</p>
<p class="p1"><span class="Apple-converted-space">            </span>&lt;/tbody&gt;</p>
<p class="p1"><span class="Apple-converted-space">        </span>&lt;/table&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;/div&gt;</p>
<p class="p1">&lt;/body&gt;</p>
<p class="p1">&lt;/html&gt;</p>
</body>
</html>
`}</HTMLBlock>