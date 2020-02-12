---
layout: page
title: 摄影
titlebar: photography
subtitle: <span class="mega-octicon octicon-flame"></span>&nbsp;&nbsp; 练就一双发现美的眼睛
menu: photography
css: ['blog-page.css']
permalink: /photography
keywords: Docker,DockerFile,Swarm,docker-machine,MCompose,Docker 学习,服务编排
---

<div class="row">

    <div class="col-md-12">

        <ul id="posts-list">
            {% for post in site.posts %}
                {% if post.category=='photography'  or post.keywords contains 'photography' or post.keywords contains 'Docker' %}
                <li class="posts-list-item">
                    <div class="posts-content">
                        <span class="posts-list-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
                        <a class="posts-list-name bubble-float-left" href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
                        <span class='circle'></span>
                    </div>
                </li>
                {% endif %}
            {% endfor %}
        </ul> 

        <!-- Pagination -->
        {% include pagination.html %}

        <!-- Comments -->
       <div class="comment">
         {% include comments.html %}
       </div>
    </div>

</div>
<script>
    $(document).ready(function(){

        // Enable bootstrap tooltip
        $("body").tooltip({ selector: '[data-toggle=tooltip]' });

    });
</script>