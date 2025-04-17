## Hi there 👋

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JLabs</title>
    <link rel="stylesheet" href="">   
</style>
</head>
<body>
    <div class="banner">
        <h1>Welcome to JLabs</h1>
    </div>
    <header>

    </header>
    <main>
    <div id="root"></div>

    </main>
    <footer>
        &copy; 2025 JLabs. All rights reserved.
    </footer>
    <script>

    /* <script src="https://code.jquery.com/jquery-3.6.0.min.js"></scrip */


                const dropdownTriggers = document.querySelectorAll('[id^="dropdown-trigger"]');
const dropdownMenus = document.querySelectorAll('[id^="dropdown-menu"]');

dropdownTriggers.forEach((trigger, index) => {
    const menu = dropdownMenus[index];

    trigger.addEventListener('click', (event) => {
        event.preventDefault();
        const isVisible = menu.style.display === 'block';
        dropdownMenus.forEach((m) => (m.style.display = 'none')); // Close other menus
        menu.style.display = isVisible ? 'none' : 'block';
    });
});

document.addEventListener('click', (event) => {
    dropdownTriggers.forEach((trigger, index) => {
        const menu = dropdownMenus[index];
        if (!trigger.contains(event.target) && !menu.contains(event.target)) {
            menu.style.display = 'none';
        }
    });
});
    </script>
</body>
</html>


<!--
**JesseDev3/JesseDev3** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
