---
layout: default
title: Главная
---

# Добро пожаловать на Minecraft Server Forum!

Здесь вы найдете всю информацию о нашем сервере и полезные гайды по игре.

- Для информации о сервере посетите раздел [Инфо](info.md)
- Для гайдов перейдите в [Гайды](guides/)

<script>
    const themeToggleBtn = document.createElement('button');
    themeToggleBtn.classList.add('theme-toggle');
    themeToggleBtn.textContent = 'Тёмная тема';
    document.body.appendChild(themeToggleBtn);

    function toggleTheme() {
        document.body.classList.toggle('dark-mode');
        if (document.body.classList.contains('dark-mode')) {
            themeToggleBtn.textContent = 'Светлая тема';
            localStorage.setItem('theme', 'dark');
        } else {
            themeToggleBtn.textContent = 'Тёмная тема';
            localStorage.setItem('theme', 'light');
        }
    }

    themeToggleBtn.addEventListener('click', toggleTheme);

    // Сохраняем выбранную тему
    const savedTheme = localStorage.getItem('theme');
    if (savedTheme === 'dark') {
        document.body.classList.add('dark-mode');
        themeToggleBtn.textContent = 'Светлая тема';
    }
</script>
