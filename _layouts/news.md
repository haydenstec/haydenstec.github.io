---
layout: default  # Use the default layout
---

<body>

    <main>
        <h1>{{ page.title }}</h1>
        {{ content }}  <!-- This will render the content of the individual news article -->
    </main>

    <footer>
        {% include footer.html %}  <!-- Include the theme's footer -->
    </footer>
</body>
