<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Our Burning Planet</title>

    <style>
        body{
            margin:0;
            font-family: Arial, Helvetica, sans-serif;
            background-color:#eef2f3;
        }

        /* ================= NAVBAR ================= */
        .navbar{
            background:#1e3c72;
            padding:15px;
            text-align:center;
            position:sticky;
            top:0;
            z-index:100;
        }
        .navbar a{
            color:white;
            text-decoration:none;
            margin:0 20px;
            font-weight:bold;
            font-size:16px;
            position:relative;
            transition:transform 0.3s;
        }
        .navbar a::after{
            content:"";
            position:absolute;
            left:0;
            bottom:-6px;
            width:0%;
            height:2px;
            background:#ffcc00;
            transition:0.3s;
        }
        .navbar a:hover{
            transform:translateY(-3px);
            color:#ffcc00;
        }
        .navbar a:hover::after{
            width:100%;
        }

        /* ================= HERO ================= */
        .hero{
            background:
                linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
                url("https://images.unsplash.com/photo-1500530855697-b586d89ba3ee");
            background-size:cover;
            background-position:center;
            color:white;
            text-align:center;
            padding:90px 20px;
        }
        .hero h1{
            font-size:44px;
            margin-bottom:15px;
            animation:fadeUp 1.2s ease forwards;
        }
        .hero p{
            font-size:20px;
            animation:fadeUp 1.2s ease forwards;
            animation-delay:0.3s;
        }

        /* ================= SECTIONS ================= */
        .section{
            max-width:1000px;
            margin:40px auto;
            padding:30px;
            background:white;
            border-radius:10px;
            box-shadow:0 4px 12px rgba(0,0,0,0.1);
            animation:fadeUp 1s ease forwards;
        }
        .section h2{
            text-align:center;
            color:#c0392b;
            margin-bottom:20px;
        }

        /* ================= TABLE ================= */
        table{
            width:100%;
            border-collapse:collapse;
            margin-top:20px;
        }
        th,td{
            border:1px solid #ccc;
            padding:12px;
            text-align:center;
        }
        th{
            background:#ff7675;
            color:white;
        }
        tr td{
            transition:background 0.3s, transform 0.2s;
        }
        tr:hover td{
            background:#dff9fb;
            transform:scale(1.02);
        }

        /* ================= LIST ================= */
        ul{
            font-size:18px;
            line-height:1.8;
        }

        /* ================= BUTTON ================= */
        .btn{
            display:block;
            margin:30px auto;
            padding:15px 40px;
            font-size:18px;
            background:#27ae60;
            color:white;
            border:none;
            border-radius:30px;
            cursor:pointer;
            animation:pulse 2s infinite;
            transition:transform 0.3s;
        }
        .btn:hover{
            transform:scale(1.1);
            background:#2ecc71;
            color:black;
        }

        /* ================= FOOTER ================= */
        .footer{
            background:#222;
            color:white;
            text-align:center;
            padding:25px;
            margin-top:40px;
        }
        .footer p{
            margin:6px 0;
            font-size:15px;
        }

        /* ================= ANIMATIONS ================= */
        @keyframes fadeUp{
            from{
                opacity:0;
                transform:translateY(40px);
            }
            to{
                opacity:1;
                transform:translateY(0);
            }
        }

        @keyframes pulse{
            0%{ transform:scale(1); }
            50%{ transform:scale(1.05); }
            100%{ transform:scale(1); }
        }
    </style>
</head>

<body>

<!-- NAVBAR -->
<div class="navbar">
    <a href="#crisis">CRISIS</a>
    <a href="#causes">CAUSES</a>
    <a href="#effects">EFFECTS</a>
    <a href="#solutions">SOLUTIONS</a>
    <a href="#act">ACT NOW</a>
</div>

<!-- HERO -->
<div class="hero">
    <h1>OUR BURNING PLANET</h1>
    <p>The Earth is heating up. Climate change is real.</p>
</div>

<!-- CRISIS -->
<div class="section" id="crisis">
    <h2>The Climate Crisis</h2>
    <p style="text-align:center;font-size:18px;">
        Global temperature has increased by <b>1.2°C</b> since 1880.
    </p>

    <table>
        <tr>
            <th>Indicator</th>
            <th>Value</th>
        </tr>
        <tr>
            <td>Temperature Rise</td>
            <td>1.2°C</td>
        </tr>
        <tr>
            <td>CO₂ Level</td>
            <td>421 ppm</td>
        </tr>
        <tr>
            <td>Sea Level Rise</td>
            <td>3.6 mm/year</td>
        </tr>
        <tr>
            <td>Arctic Ice Loss</td>
            <td>13%</td>
        </tr>
    </table>
</div>

<!-- CAUSES -->
<div class="section" id="causes">
    <h2>Causes of Global Warming</h2>
    <ul>
        <li>Burning of fossil fuels</li>
        <li>Deforestation</li>
        <li>Industrial pollution</li>
        <li>Transportation emissions</li>
        <li>Over-consumption</li>
    </ul>
</div>

<!-- EFFECTS -->
<div class="section" id="effects">
    <h2>Effects on Earth</h2>
    <ul>
        <li>Rising sea levels</li>
        <li>Extreme weather conditions</li>
        <li>Loss of wildlife</li>
        <li>Food and water shortages</li>
        <li>Health risks</li>
    </ul>
</div>

<!-- SOLUTIONS -->
<div class="section" id="solutions">
    <h2>Possible Solutions</h2>
    <ul>
        <li>Use renewable energy</li>
        <li>Plant more trees</li>
        <li>Reduce plastic usage</li>
        <li>Save electricity</li>
        <li>Support climate policies</li>
    </ul>
</div>

<!-- ACT -->
<div class="section" id="act">
    <h2>Act Now</h2>
    <p style="text-align:center;font-size:18px;">
        Every action counts. The future is in our hands.
    </p>
    <button class="btn">Take Action</button>
</div>

<!-- FOOTER -->
<div class="footer">
    <p><b>Contact Us</b></p>
    <p>📞 Mobile: 8520852085</p>
    <p>📧 Email: globalwarming@gmail.com</p>
    <p>Climate Data: NASA | IPCC | NOAA</p>
    <p>© Our Planet Project</p>
</div>

</body>
</html>
