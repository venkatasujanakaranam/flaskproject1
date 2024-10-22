#index.html
<title> User Form</title>
User Information Form
Username:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>User Information Form</title>
    <link rel="stylesheet" href="{{ url_for('static', filename='css/style.css') }}">
    <script src="{{ url_for('static', filename='js/script.js') }}" defer></script>
</head>
<body>
    <div class="form-container">
        <h1>User Information Form</h1>
        <form action="/" method="POST" id="userForm" onsubmit="return validateForm()">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" required><br>

            <label for="phone">Phone:</label>
            <input type="tel" id="phone" name="phone" required><br>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required><br>

            <input type="submit" value="Submit">
        </form>
        <p id="error-msg" class="error"></p>
    </div>
</body>
</html>
