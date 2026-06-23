1.How template inheritance works in my project-

In my project, I used Django template inheritance to avoid repeating the same HTML code on multiple pages. I created a base.html file that contains the common layout such as header and page structure. Then home.html and about.html extend the base template using {% extends 'base.html' %}.
This makes the project more organized, reusable, and easier to maintain.

2.Why I chose specific filters and tags-

I used Django template filters and tags to display dynamic data in a better format.
Filters used:
|title → converts text into title case
|upper → converts text into uppercase
Tags used:
{% for %} → used to loop through tasks
{% empty %} → shows a message when no tasks are available
{% block %} → used for template inheritance
These features make the templates dynamic and user-friendly.

3.How data flows from views to templates-

In Django, data flows from views to templates using context dictionaries. The view function collects data from the database and sends it to the template.
