# aball2025hellenthal<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dienstplan Abfallentsorgung 2025</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; }
        table { width: 80%; margin: 20px auto; border-collapse: collapse; }
        th, td { border: 1px solid black; padding: 10px; }
        th { background-color: #f2f2f2; }
        button { padding: 5px 10px; cursor: pointer; }
    </style>
</head>
<body>
    <h2>Dienstplan Abfallentsorgung 2025</h2>
    <table>
        <thead>
            <tr>
                <th>Datum</th>
                <th>Wochentag</th>
                <th>Abfallart</th>
                <th>Mitarbeiter</th>
                <th>Aktion</th>
            </tr>
        </thead>
        <tbody id="plan-body"></tbody>
    </table>

    <script>
        const termine = [
            { datum: "01.01.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "08.01.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "15.01.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "22.01.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "29.01.2025", tag: "Mittwoch", abfall: "Gelber Sack" },
            { datum: "05.02.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "12.02.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "19.02.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "26.02.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "05.03.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "12.03.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "19.03.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "26.03.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "02.04.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "09.04.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "16.04.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "23.04.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "30.04.2025", tag: "Mittwoch", abfall: "Gelber Sack" },
            { datum: "07.05.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "14.05.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "21.05.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "28.05.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "04.06.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "11.06.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "18.06.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "25.06.2025", tag: "Mittwoch", abfall: "Papier" },
            { datum: "02.07.2025", tag: "Mittwoch", abfall: "Restmüll" },
            { datum: "09.07.2025", tag: "Mittwoch", abfall: "Papier"
