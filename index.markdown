---
layout: page
---

<div class="courselist">
{% for course in site.courses %}
    <div class="coursecard">
        <div class="deptandinst">
            <span class="dept"> {{course.department}} </span> &nbsp; | &nbsp; <span class="inst">{{course.instructor}}</span>
        </div>
        <div class="coursedetail">
            <div style="font-size:25px; color:black;" >{{course.title}}: {{course.name}}</div>
        </div>
        <div class="LTPC">
            <span class="lec"><i class="fa-solid fa-chalkboard-user"></i> {{course.lectures}} Lectures </span>
            <span class="tut"><i class="fa-solid fa-comment-dots"></i> {{course.tutorials}} Tutorials </span>
            <span class="pra"><i class="fa-solid fa-flask"></i> {{course.practicals}} Practicals </span>
            <span class="cre"><i class="fa-solid fa-graduation-cap"></i> {{course.credits}} Credits </span>
        </div>
        <div class="desc">{{course.description}}</div>
        <!-- <div class="knowmore"><a href="{{course.url | relative_url}}">Know more</a></div> -->
        <a href="{{course.url | relative_url}}"><button type="button" class="btn btn-info knowmore">Know more</button></a>
    </div>
{% endfor %}
</div>

