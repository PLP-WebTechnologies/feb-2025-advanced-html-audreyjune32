<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        form {
            width: 50%;
            margin: auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        fieldset {
            border: 2px saddlebrown snow;
            padding: 15px;
        }
        legend {
            font-weight: bold;
            font-size: 1.2em;
            color:black;
        }
        label {
            margin-top: 10px;
            display: block;
        }
        input, select, textarea {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .form-section {
            margin-bottom: 20px;
        }
        .radio-group, .checkbox-group {
            margin-top: 10px;
        }
    </style>
</head>
<body>

    <h1>Registration Form</h1>
    <form action="/submit-form" method="POST">
        <!-- Personal Information Section -->
        <fieldset>
            <legend>Personal Information</legend>
            
            <!-- Name Field -->
            <div class="form-section">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>
            </div>

            <!-- Email Field -->
            <div class="form-section">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>
            </div>

            <!-- Password Field -->
            <div class="form-section">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" placeholder="Enter your password" required minlength="8">
            </div>

            <!-- Date of Birth Field -->
            <div class="form-section">
                <label for="dob">Date of Birth:</label>
                <input type="date" id="dob" name="dob" required>
            </div>
        </fieldset>

        <!-- Gender Section -->
        <fieldset>
            <legend>Gender</legend>
            
            <!-- Radio Buttons for Gender -->
            <div class="radio-group">
                <input type="radio" id="male" name="gender" value="male" required>
                <label for="male">Male</label>

                <input type="radio" id="female" name="gender" value="female">
                <label for="female">Female</label>

                <input type="radio" id="other" name="gender" value="other">
                <label for="other">Other</label>
            </div>
        </fieldset>

        <!-- Course Section -->
        <fieldset>
            <legend>Course</legend>
            
            <!-- Dropdown Menu -->
            <div class="form-section">
                <label for="preferences">Select your Course:</label>
                <select id="preferences" name="preferences" required>
                    <option value="">Choose your Course</option>
                    <option value="Course">computer science</option>
                    <option value="">Information technology</option>
                    <option value="">ICT</option>
                </select>
            </div>

            <!-- Checkbox Group -->
            <div class="checkbox-group">
                <input type="checkbox" id="terms" name="terms" required>
                <label for="terms">I agree to the <a href="#">terms and conditions</a></label>

                <input type="checkbox" id="privacy" name="privacy" required>
                <label for="privacy">I agree to the <a href="#">privacy policy</a></label>
            </div>
        </fieldset>

        <!-- Submit Button -->
        <div class="form-section">
            <input type="submit" value="Register">
        </div>
    </form>

</body>
</html>
