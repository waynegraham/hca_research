---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<h1>Full List</h1>
<ol>
 {% for member in site.data.aau_members %}
    <li>
        <a href="{{member.website}}">{{ member.institution }}</a>
    </li>
    {% endfor %}
    {% for member in site.data.hbcu_members %}
    <li>
        {{ member.institution }}
    </li>
    {% endfor %}
    {% for member in site.data.cenl_members %}
    <li>
        {{ member.institution }}
    </li>
    {% endfor %}
    {% for member in site.data.rfn_members %}
    <li>
        {{ member.institution }} ({{ member.country }})
    </li>
    {% endfor %}
    {% for member in site.data.clir_members %}
    <li>
        {{ member.institution }}
    </li>
    {% endfor %}
</ol>

<h2>AAU Members</h2>
<ol>
    {% for member in site.data.aau_members %}
    <li>
        <a href="{{member.website}}">{{ member.institution }}</a>
    </li>
    {% endfor %}
</ol>

<h2>HBCU Members</h2>
<ol>
   {% for member in site.data.hbcu_members %}
    <li>
        {{ member.institution }}
    </li>
    {% endfor %}
</ol>

<h2>CENL Members</h2>
<ol>
   {% for member in site.data.cenl_members %}
    <li>
        {{ member.institution }}
    </li>
    {% endfor %}
</ol>

<h2>RFN Members</h2>
<ol>
   {% for member in site.data.rfn_members %}
    <li>
        {{ member.institution }} ({{ member.country }})
    </li>
    {% endfor %}
</ol>

<h2>CLIR Members</h2>
<ol>
   {% for member in site.data.clir_members %}
    <li>
        {{ member.institution }}
    </li>
    {% endfor %}
</ol>