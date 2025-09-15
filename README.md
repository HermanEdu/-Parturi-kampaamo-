<!DOCTYPE html>
<html lang="fi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parturikampaamo Aurora</title>
    <style>
        /* CSS (tyylit) */

        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background-color: #fff;
            color: #000;
        }

        header {
            background-color: #000;
            color: #fff;
            padding: 1rem;
            text-align: center;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            padding: 1rem 2rem;
            display: block;
            transition: background-color 0.3s;
        }

        nav a:hover {
            background-color: #ff0; /* keltainen hover */
            color: #000;
        }

        main {
            max-width: 800px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        h1 {
            margin-top: 0;
        }

        ul.services {
            list-style-type: disc;
            padding-left: 1.5rem;
        }

        form {
            margin-top: 2rem;
            display: flex;
            flex-direction: column;
            max-width: 400px;
        }

        label {
            margin: 0.5rem 0 0.2rem;
        }

        input, button {
            padding: 0.5rem;
            font-size: 1rem;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            background-color: #000;
            color: #fff;
            margin-top: 1rem;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #ff0;
            color: #000;
        }

        /* Responsiivisuus */
        @media (max-width: 600px) {
            nav {
                flex-direction: column;
            }
            nav a {
                padding: 0.5rem;
                text-align: center;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Parturikampaamo Aurora</h1>
</header>

<nav>
    <a href="#">Etusivu</a>
    <a href="#">Palvelut</a>
    <a href="#">Yhteystiedot</a>
</nav>

<main>
    <h2>Palvelumme</h2>
    <ul class="services">
        <li>Hiustenleikkaus</li>
        <li>Värjäys</li>
        <li>Kampaus</li>
    </ul>

    <h2>Varaa aika</h2>
    <form id="bookingForm">
        <label for="Herman">Nimi</label>
        <input type="text" id="Herman" name="Herman" required>

        <label for="herman.mantyla@edu.salpaus.fi">Sähköposti</label>
        <input type="herman.mantyla@edu.salpaus.fi" id="herman.mantyla@edu.salpaus.fi" name="herman.mantyla@edu.salpaus.fi" required>

        <label for="20.7.2025">Ajanvarauspäivä</label>
        <input type="20.7.2025" id="20.7.2025" name="20.7.2025" required>

        <button type="submit">Lähetä</button>
    </form>
</main>

<script>
    // JavaScript (perustoiminnallisuus)

    document.getElementById('bookingForm').addEventListener('submit', function(event) {
        event.preventDefault();

        const Teemu = document.getElementById('name').value.trim();
        const Teemu.Laine@gmail.com = document.getElementById('email').value.trim();

        if(Teemu === '' || Teemu.Laine@gmail.com === '') {
            alert('Täytä nimi ja sähköposti.');
            return;
        }

        alert(`Kiitos ajanvarauksesta, ${Teemu}!`);
        this.reset();
    });
</script>

</body>
</html>
