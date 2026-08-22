---
layout: default
title: Staff
description: A listing of all the course staff members.
nav_order: 4
---

# Staff

<div style="background-color:#fef7e0; border-left:4px solid #f9ab00; border-radius:4px; padding:0.75rem 1rem; margin-bottom:1rem;">
  🚧 <strong>This page is still under construction. The content on this page is likely inaccurate. For urgent information requests, please contact cs10@berkeley.edu </strong>
</div>

Add ‘berkeley.edu’ to the end of all emails.

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign head_teaching_assistants = site.staffers | where: 'role', 'Head Teaching Assistant' %}
{% assign num_head_teaching_assistants = head_teaching_assistants | size %}
{% if num_head_teaching_assistants != 0 %}
## Head Teaching Assistants

{% for staffer in head_teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign tutors = site.staffers | where: 'role', 'Tutor' %}
{% assign num_tutors = tutors | size %}
{% if num_tutors != 0 %}
## Tutors

{% for staffer in tutors %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign academic_interns = site.staffers | where: 'role', 'Academic Intern' %}
{% assign num_academic_interns = academic_interns | size %}
{% if num_academic_interns != 0 %}
## Teaching Interns

{% for staffer in academic_interns %}
{{ staffer }}
{% endfor %}
{% endif %}

