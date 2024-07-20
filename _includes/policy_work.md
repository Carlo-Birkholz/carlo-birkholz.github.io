<h2 id="publications" style="margin: 2px 0px -15px;">Policy Work</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.policy_work.main %}

<li>
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}" target="_blank">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.contractor }}</em> </div>
  </div>
</div>
    {% if link.abstract %}
    <details style="position: relative;padding-right: 15px;padding-left: 15px;"><summary>Project description</summary><div style="text-align: justify">{{link.abstract}}</div></details>
    {% endif %}
    {% if link.output %}
    <div style="position: relative;padding-right: 15px;padding-left: 15px;"><br>Project output: <div style="color: rgb(62, 183, 240); font-weight: bold"> {{link.output}} </div> 
    <div class="links">    
    <a href="{{ link.output1 }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Update April 2023</a>
    <a href="{{ link.output2 }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Update June 2022</a>
    <a href="{{ link.output3 }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Update December 2021</a> </div> </div>
    {% endif %}
    {% if link.paper_output %}
      <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;"><br>Project output:
        <div class="title"><a href="{{ link.pdf1 }}" target="_blank">{{ link.paper1 }}</a></div>
        <div class="author">{{ link.authors1 }}</div>
        <div class="periodical"><em>{{ link.journal1 }}</em> 
      </div>
        <div class="links">
        {% if link.pdf1 %} 
            <a href="{{ link.pdf1 }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
        {% endif %}
        </div>
        </div>
        {% if link.abstract1 %}
        <details style="position: relative;padding-right: 15px;padding-left: 15px;"><summary>Abstract</summary><div style="text-align: justify">{{link.abstract1}}</div></details>
        {% endif %}
        #<div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;"><br>
        <div class="title"><a href="{{ link.pdf2 }}" target="_blank">{{ link.paper2 }}</a></div>
        <div class="author">{{ link.authors2 }}</div>
        <div class="periodical"><em>{{ link.journal2 }}</em></div>
        {% if link.notes2 %} 
        <strong> <i style="color:#e74d3c">{{ link.notes2 }}</i></strong>
        {% endif %}
        <div class="links">
        {% if link.pdf2 %} 
            <a href="{{ link.pdf2 }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
        {% endif %}
        </div>
        </div>
        {% if link.abstract2 %}
        <details style="position: relative;padding-right: 15px;padding-left: 15px;"><summary>Abstract</summary><div style="text-align: justify">{{link.abstract2}}</div></details>
    {% endif %}
</li>

<br>

{% endfor %}

</ol>
</div>
