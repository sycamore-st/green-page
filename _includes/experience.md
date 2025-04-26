<h2 id="experience" style="margin: 2px 0px -15px;">Working Experience</h2>

{% for job in site.data.experience.main %}
<h3>{{ job.company }} – {{ job.location }}</h3>
<div style="margin-left: 20px;">
    {% for role in job.roles %}
    <p><strong>{{ role.title }}</strong><br><em>{{ role.duration }}</em></p>
    <ul>
        {% for item in role.responsibilities %}
        <li>{{ item }}</li>
        {% endfor %}
    </ul>
    {% endfor %}
</div>
{% endfor %}