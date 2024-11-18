<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Flirt Master VIP - Tailored flirtatious messages for your love life!">
    <title>Flirt Master VIP</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #ff7eb3, #ff758c);
            color: #fff;
            text-align: center;
        }
        header {
            background: #ff477e;
            padding: 1rem 0;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        header h1 {
            margin: 0;
            font-size: 2rem;
        }
        .form-container {
            margin: 2rem auto;
            padding: 2rem;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 8px;
            max-width: 500px;
        }
        .form-container label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
        }
        .form-container input, .form-container select, .form-container button {
            width: 100%;
            padding: 0.8rem;
            margin-bottom: 1rem;
            border: none;
            border-radius: 4px;
            font-size: 1rem;
        }
        .form-container button {
            background: #ff477e;
            color: #fff;
            cursor: pointer;
        }
        .form-container button:hover {
            background: #ff295b;
        }
        footer {
            margin-top: 2rem;
            padding: 1rem;
            background: #ff477e;
        }
    </style>
</head>
<body>
    <header>
        <h1>Flirt Master VIP</h1>
    </header>

    <div class="form-container">
        <h2>Create Flirtatious Messages</h2>
        <form id="flirt-form">
            <label for="gender">I am:</label>
            <select id="gender" required>
                <option value="male">Male</option>
                <option value="female">Female</option>
            </select>

            <label for="age">My Age:</label>
            <input type="number" id="age" min="18" max="100" required>

            <label for="preference">Looking to flirt with:</label>
            <select id="preference" required>
                <option value="male">Males</option>
                <option value="female">Females</option>
                <option value="everyone">Everyone</option>
            </select>

            <button type="submit">Generate Flirt Messages</button>
        </form>

        <div id="result" style="margin-top: 1rem;"></div>
    </div>

    <footer>
        <p>&copy; 2024 Flirt Master VIP. All Rights Reserved.</p>
    </footer>

    <script>
        document.getElementById("flirt-form").addEventListener("submit", function(event) {
            event.preventDefault();
            const gender = document.getElementById("gender").value;
            const age = document.getElementById("age").value;
            const preference = document.getElementById("preference").value;

            // Generate mock flirt messages (replace with API calls for real responses)
            const messages = {
                male: "Hey, handsome! How's it going?",
                female: "Hello, gorgeous! You just made my day!",
                everyone: "You're simply stunning. Let's chat!"
            };

            document.getElementById("result").innerText =
                `Flirty Message for you: ${messages[preference] || "Hello there!"}`;
        });
    </script>
</body>
</html>

