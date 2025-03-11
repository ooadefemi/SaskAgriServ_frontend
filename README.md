# SaskAgriServ_frontend
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Farmer Data Portal</title>
    <script defer src="script.js"></script>
    <style>
        body { font-family: Arial, sans-serif; margin: 20px; }
        table { width: 100%; border-collapse: collapse; margin-top: 20px; }
        th, td { border: 1px solid black; padding: 10px; text-align: left; }
        th { background-color: #f4f4f4; }
    </style>
</head>
<body>

    <h2>Farmer Data Portal</h2>

    <h3>Add Farmer</h3>
    <form id="farmerForm">
        <label for="emailid">Email ID:</label>
        <input type="text" id="emailid" required><br><br>
        
        <label for="name">Name:</label>
        <input type="text" id="name" required><br><br>

        <label for="age">Age:</label>
        <input type="number" id="age" required><br><br>

        <button type="submit">Add Farmer</button>
    </form>

    <h3>Farmer List</h3>
    <button onclick="fetchFarmers()">Refresh List</button>
    <table>
        <thead>
            <tr>
                <th>Email ID</th>
                <th>Name</th>
                <th>Age</th>
            </tr>
        </thead>
        <tbody id="farmerTableBody"></tbody>
    </table>

</body>
</html>
