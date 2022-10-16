---

layout: frontpage
header:
  image_fullwidth:
title: "MADHAV Lab - Indian Institute of Technology Kanpur"

sidebar: right

permalink: /index.html
homepage: true

---

<div class="row" style= "margin-top: 30px; margin-left: 1%">
    <div class="light-section mt-6 mb-6">
      <h3 class="section-title">Breaking News</h3>
      <ul class="timeline col-md-6 off-md-6">
        {% assign news = site.news | sort: "timestamp" | reverse %}
        {% for n in news %}
          {% if n.show_on_index %}
            {% include news_item.html news_date=n.news_date title=n.title year=n.year news_content=n.news_content %}
          {% endif %}
        {% endfor %}
      </ul>
  </div>
</div>



<div class="pc dark-section" style="">
  <br>
  <h3 class="section-title"> About TVG </h3> 

Our group’s research interests lie at the intersection of the theory and application of machine learning - with a focus on applications in audio and speech processing, Physics and Music. With a strong interest in the mathematical fundamentals and a passion for real-world application, our group aims on being at the forefront of the field, by carrying out impactful research in the areas of deep learning, machine learning and speech processing, guided by application contexts derived from real-world use. 

Members of the group have also contributed significantly in a variety of research directions. We have collaborated with many exciting high tech companies, institutes and organizations including Google, Samsung, Prasar Bharti, MIT, and DST-GOI.

</div>


<div class="pc light-section" style="">
  <br>
  <h3 class="section-title"> Join the Lab </h3> 

  We are currently looking to hire talented post docs and doctoral students, please check the <a href="https://torrvision.com/recruitment/"> recruitment page </a> for more details .

</div>
