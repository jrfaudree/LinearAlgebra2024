{% assign data = include.data %}
<table class="asst-table">
{% for ws in data.quizexam %}
<tr>
	<td>{{ ws.name }}</td>
	<td>
		<table class="inner">
			{% if ws.notes %}
		  <tr>
			    <td><a href="{{ data.home }}/{{ ws.notes }}">notes</a></td>
			</tr>
			{% endif %}
			{% if ws.blank %}
		  <tr>
			    <td><a href="{{ data.home }}/{{ ws.blank }}">blank</a></td>
			</tr>
			{% endif %}
			{% if ws.solutions %}
			<tr>
			    <td><a href="{{ data.home }}/{{ ws.solutions }}">solutions</a></td>
			</tr>
			{% endif %}
			{% if ws.file %}
		  <tr>
			    <td><a href="{{ data.home }}/{{ ws.file }}">Matlab code</a></td>
			</tr>
			{% endif %}
			{% if ws.image %}
		  <tr>
			    <td><a href="{{ data.home }}/{{ ws.image }}">output image</a></td>
			</tr>
			{% endif %}