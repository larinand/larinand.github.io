---
layout: default
title: Home
---

<!-- # Selamat datang di blog saya 👋 -->

<!-- Ini adalah blog sederhana berbasis Markdown. -->

<!-- ## New Article -->

<!-- - [Hello World]({{ site.baseurl }}/2026/04/13/hello-world/) -->

<!-- <ul>
{% for post in site.posts %}
    <li>
        <a href="{{site.baseurl}}{{ post.url }}">{{ post.title }}</a>
    </li>
{% endfor %}
</ul> -->

<ul style="list-style: none; padding: 0;">
{% for post in site.posts %}

    <li style="margin-bottom: 20px;">

        <!-- Baris judul + bahasa -->
        <div style="display: flex; align-items: center; gap: 20px;">

            <!-- Bahasa -->
            <span style="font-size: 20px; color: #888;">
            {{ post.language }}
            </span>

            <div>
                <!-- Judul -->
                <a href="{{ site.baseurl }}{{ post.url }}"
                style="font-size: 20px; font-weight: 500; text-decoration: none; color: #333;"
                onmouseover="this.style.textDecoration='underline'"
                onmouseout="this.style.textDecoration='none'">
                {{ post.title }}
                </a>

                <!-- Tanggal -->
                <div style="font-size: 14px; color: #888; margin-top: 5px;">
                    {{ post.date | date: "%b %d, %Y" }}
                </div>
            </div>

        </div>

    </li>

{% endfor %}

</ul>
