<div class="container--inner">
    
      <div aria-label="Question Content" class="challenge-text hrx-version ck_table-wrap fadeinContent" style="min-height:100px;"><style type="text/css">.ps-content-wrapper-v0 div { margin: 0 auto; overflow: auto; } .ps-content-wrapper-v0 div.preheader { display: none; } .ps-content-wrapper-v0 p { white-space: pre-wrap; padding-left: 4px; padding-right: 4px; padding-top: 0px; padding-bottom: 2px; } .ps-content-wrapper-v0 p.section-title { font-weight: bold; padding-bottom: 0px; } .ps-content-wrapper-v0 ol.plain-list, .ps-content-wrapper-v0 ul.plain-list { list-style-type: none; padding: 4px; } .ps-content-wrapper-v0 li { white-space: normal; margin-top: 4px; margin-bottom: 4px; } .ps-content-wrapper-v0 code { color: black; } .ps-content-wrapper-v0 pre { background-color: #f4faff; border: 0; border-radius: 2px; margin: 8px; padding: 10px; } .ps-content-wrapper-v0 figure { background-color: transparent; display: table; margin-top: 8px; margin-bottom: 8px; text-align: center; margin-left: auto; margin-right: auto; } .ps-content-wrapper-v0 figcaption { text-align: center; display: table-caption; caption-side: bottom; margin-top: 4px; margin-bottom: 4px; } .ps-content-wrapper-v0 img { width: auto; max-width: 100%; height: auto; } .ps-content-wrapper-v0 details { background-color: transparent; padding-left: 4px; padding-right: 4px; padding-top: 0px; padding-bottom: 2px; } .ps-content-wrapper-v0 details details { padding-left: 8px; padding-right: 8px; } .ps-content-wrapper-v0 details summary { background-color: #39424e; color: white; font-weight: bold; margin-top: 4px; margin-bottom: 4px; padding: 8px; } .ps-content-wrapper-v0 details details summary code { color: black; font-weight: bold; padding-left: 2px; padding-right: 2px; padding-top: 4px; padding-right: 4px; margin-left: 4px; } .ps-content-wrapper-v0 details div.collapsable-details { margin: 0 auto; padding-left: 4px; padding-right: 4px; padding-top: 0px; padding-bottom: 2px; overflow: auto; } .ps-content-wrapper-v0 details div.collapsable-details pre { margin-left: 4px; margin-right: 4px; margin-top: 4px; margin-bottom: 4px; } .ps-content-wrapper-v0 table { border: 1px solid black; border-collapse: collapse; border-color: darkgray; margin: 0 auto; margin-top: 8px; margin-bottom: 8px; padding: 8px; width: 96%; table-layout: fixed; } .ps-content-wrapper-v0 table tbody tr th, .ps-content-wrapper-v0 table tbody tr td { font-weight: bold; white-space: nowrap; text-align: center; vertical-align: middle; border: 1px solid black; border-color: darkgray; padding: 8px; } .ps-content-wrapper-v0 table tbody tr th.description { width: 60%; } .ps-content-wrapper-v0 table tbody tr td { font-weight: normal; white-space: normal; } .ps-content-wrapper-v0 table.function-params tbody tr:first-child td.headers { border-bottom-width: 2px; } .ps-content-wrapper-v0 table.function-params tbody tr:last-child td { border-top-width: 2px; border-top-color: darkgray; } .ps-content-wrapper-v0 table.function-params tbody tr td.headers { width: 25%; font-weight: bold; text-align: center; border: 1px solid black; border-right-width: 2px; border-color: darkgray; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell { width: 100%; height: 100%; padding: 0px; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table { width: 100%; height: 100%; padding: 0px; margin: 0px; border: 0; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table tbody tr td.code { white-space: normal; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table tbody tr th { border-top: 0; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table tbody tr th:first-child { border-left: 0; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table tbody tr th:last-child { border-right: 0; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table tbody tr:last-child td { border-bottom: 0; border-top-width: 1px; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table tbody tr td:first-child { border-left: 0; } .ps-content-wrapper-v0 table.function-params tbody tr td.params-table-cell table.params-table tbody tr td:last-child { border-right: 0; } .ps-content-wrapper-v0 .left { text-align: left; } .ps-content-wrapper-v0 .right { text-align: right; } .ps-content-wrapper-v0 .code { font-family: monospace; white-space: nowrap; } .ps-content-wrapper-v0 .json-object-array ol, .ps-content-wrapper-v0 .json-object-array ol ul { margin-top: 0px; padding-left: 14px; } .json-object-array li { float: left; margin-right: 30px; margin-left: 10px; } .json-object-array pre { padding: 4px; margin-left: 0px; }
</style>
<div class="ps-content-wrapper-v0">
<p>In this challenge, you are part of a team building a git event tracking platform. One requirement is for a REST API service to provide events information using the Spring Boot framework. You will need to add functionality to add and delete information as well as to perform some queries. You'll be dealing with typical information for git event data like repository, actor, event type, etc. The team has come up with a set of requirements including filtering and ordering requirements, response codes and error messages for the queries you must implement.</p>

<p>&nbsp;</p>

<p>The definitions and a detailed requirements list follow. You will be graded on whether your application performs data retrieval and manipulation based on given use cases exactly as described in the requirements.</p>

<p>&nbsp;</p>

<p>Each event data is a JSON entry with the following keys:</p>

<ul>
	<li>
<code>id</code>: This is the event unique ID.</li>
	<li>
<code>type</code>: This is the event type.</li>
	<li>
<code>actor</code>: The actor responsible for the event. The actor itself is a JSON entry consisting of following fields:
	<ul>
		<li>
<code>id</code>: This is the actor unique ID.</li>
		<li>
<code>login</code>: This is the actor unique login ID.</li>
		<li>
<code>avatar_url</code>: This is the actor avatar URL.</li>
	</ul>
	</li>
	<li>
<code>repo</code>: The repository to which this event is associated with. The repo itself is a JSON entry consisting of following fields:
	<ul>
		<li>
<code>id</code>: This is the repo unique ID.</li>
		<li>
<code>name</code>: This is the repo name.</li>
		<li>
<code>url</code>: This is the repo URL.</li>
	</ul>
	</li>
	<li>
<code>created_at</code>: This is the timestamp for the event creation given in the format <code>yyyy-MM-dd HH:mm:ss</code>. The timezone is <code>UTC +0</code>.</li>
</ul>

<p>&nbsp;</p>

<details><summary class="section-title">Sample JSON git event object</summary>

<div class="collapsable-details">
<pre>{
&nbsp; "id":3761013629,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":2301944,
&nbsp; &nbsp; "login":"williamssue",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2301944"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":363748,
&nbsp; &nbsp; "name":"michael73/maxime-nisi-hic",
&nbsp; &nbsp; "url":"https://github.com/michael73/maxime-nisi-hic"
&nbsp; },
&nbsp; "created_at":"2015-06-25 09:13:31"
}</pre>
</div>
</details>

<p>&nbsp;</p>

<p>The <em>REST</em> service should implement the following functionalities:</p>

<ol>
	<li>
<em>Erasing all the events</em>: The service should be able to erase all the events by the <em>DELETE</em> request at <code>/erase</code>. The <em>HTTP</em> response code should be <em>200</em>.</li>
	<li>
<em>Adding new events</em>: The service should be able to add a new event by the <em>POST</em> request at <code>/events</code>. The event <em>JSON</em> is sent in the request body. If an event with the same id already exists then the <em>HTTP</em> response code should be <em>400</em>, otherwise, the response code should be <em>201</em>.</li>
	<li>
<em>Returning all the events</em>: The service should be able to return the JSON array of all the events by the <em>GET</em> request at <code>/events</code>. The <em>HTTP</em> response code should be <em>200</em>. The JSON array should be sorted in ascending order by event ID.</li>
	<li>
<em>Returning the event records filtered by the actor ID</em>: The service should be able to return the <em>JSON</em> array of all the events which are performed by the actor ID by the <em>GET</em> request at <code>/events/actors/{actorID}</code>. If the requested actor does not exist then <em>HTTP</em> response code should be <em>404</em>, otherwise, the response code should be <em>200</em>. The JSON array should be sorted in ascending order by event ID.</li>
	<li>
<em>Updating the avatar URL of the actor</em>: The service should be able to update the avatar URL of the actor by the <em>PUT</em> request at <code>/actors</code>. The actor <em>JSON</em> is sent in the request body. If the actor with the id does not exist then the response code should be <em>404</em>, or if there are other fields being updated for the actor then the <em>HTTP</em> response code should be <em>400</em>, otherwise, the response code should be <em>200</em>.</li>
	<li>
<em>Returning the actor records ordered by the total number of events</em>: The service should be able to return the <em>JSON</em> array of all the actors sorted by the total number of associated events with each actor in descending order by the <em>GET</em> request at <code>/actors</code>. If there are more than one actors with the same number of events, then order them by the timestamp of the latest event in the descending order. If more than one actors have the same timestamp for the latest event, then order them by the alphabetical order of login. The <em>HTTP</em> response code should be <em>200</em>.</li>
</ol>

<p>&nbsp;</p>

<p>You should complete the given incomplete project so that it passes all the test cases when running the provided <em>JUnit</em> tests. The project by default supports the use of H2 database, but you can make use of any database to store the weather data by specifying the dependency in the <em>pom.xml</em> file.</p>

<p>&nbsp;</p>

<details><summary class="section-title">Sample Series of Requests</summary>

<div class="collapsable-details">
<p>Requests are received in the following order and are provided in the test file <em>http00.json</em>:</p>

<details><summary class="section-title">POST <code>/events</code></summary>

<div class="collapsable-details">
<p>Consider the following <em>POST</em> requests (these are performed in the ascending order of event id):</p>

<div class="json-object-array">
<ol>
	<li>
	<pre>{
&nbsp; "id":3761013629,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":2301944,
&nbsp; &nbsp; "login":"williamssue",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2301944"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":363748,
&nbsp; &nbsp; "name":"michael73/maxime-nisi-hic",
&nbsp; &nbsp; "url":"https://github.com/michael73/maxime-nisi-hic"
&nbsp; },
&nbsp; "created_at":"2015-06-25 09:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":2226511299,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":1834821,
&nbsp; &nbsp; "login":"carrie89",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/1834821"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":332247,
&nbsp; &nbsp; "name":"carrie89/quod-maxime-dolorum",
&nbsp; &nbsp; "url":"https://github.com/carrie89/quod-maxime-dolorum"
&nbsp; },
&nbsp; "created_at":"2014-02-05 11:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":3077377593,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":4933705,
&nbsp; &nbsp; "login":"davistravis",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/4933705"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":103403,
&nbsp; &nbsp; "name":"ngarcia/pariatur",
&nbsp; &nbsp; "url":"https://github.com/ngarcia/pariatur"
&nbsp; },
&nbsp; "created_at":"2014-11-13 22:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":1706531305,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":2559288,
&nbsp; &nbsp; "login":"upratt",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2559288"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":369757,
&nbsp; &nbsp; "name":"upratt/maxime-cum-optio-a",
&nbsp; &nbsp; "url":"https://github.com/upratt/maxime-cum-optio-a"
&nbsp; },
&nbsp; "created_at":"2013-08-17 11:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":1351371245,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":1880228,
&nbsp; &nbsp; "login":"joshua15",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/1880228"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":442361,
&nbsp; &nbsp; "name":"joshua15/maiores-aspernatur",
&nbsp; &nbsp; "url":"https://github.com/joshua15/maiores-aspernatur"
&nbsp; },
&nbsp; "created_at":"2013-04-26 11:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":3541994625,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":2132248,
&nbsp; &nbsp; "login":"robert02",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2132248"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":293914,
&nbsp; &nbsp; "name":"thomasjones/dolorem-architecto",
&nbsp; &nbsp; "url":"https://github.com/thomasjones/dolorem-architecto"
&nbsp; },
&nbsp; "created_at":"2015-04-07 19:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":4803136235,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":4108139,
&nbsp; &nbsp; "login":"fcoleman",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/4108139"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":462411,
&nbsp; &nbsp; "name":"yfrazier/sit-fuga-aut-earum",
&nbsp; &nbsp; "url":"https://github.com/yfrazier/sit-fuga-aut-earum"
&nbsp; },
&nbsp; "created_at":"2016-07-02 22:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":3587954242,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":3271833,
&nbsp; &nbsp; "login":"philip55",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/3271833"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":322322,
&nbsp; &nbsp; "name":"philip55/architecto",
&nbsp; &nbsp; "url":"https://github.com/philip55/architecto"
&nbsp; },
&nbsp; "created_at":"2015-04-25 18:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":1724643219,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":2659286,
&nbsp; &nbsp; "login":"larry92",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2659286"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":198663,
&nbsp; &nbsp; "name":"larry92/dignissimos",
&nbsp; &nbsp; "url":"https://github.com/larry92/dignissimos"
&nbsp; },
&nbsp; "created_at":"2013-08-24 00:13:31"
}</pre>
	</li>
	<li>
	<pre>{
&nbsp; "id":2707150273,
&nbsp; "type":"PushEvent",
&nbsp; "actor":{
&nbsp; &nbsp; "id":1233932,
&nbsp; &nbsp; "login":"arielchapman",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/1233932"
&nbsp; },
&nbsp; "repo":{
&nbsp; &nbsp; "id":481585,
&nbsp; &nbsp; "name":"brianramos/quam-unde-illo",
&nbsp; &nbsp; "url":"https://github.com/brianramos/quam-unde-illo"
&nbsp; },
&nbsp; "created_at":"2014-07-11 15:13:31"
}</pre>
	</li>
</ol>
</div>
</div>
</details>

<details><summary class="section-title">GET <code>/events/actors/1233932</code></summary>

<div class="collapsable-details">
<p>The response of the <em>GET</em> request is the following <em>JSON</em> array with the <em>HTTP</em> response code <em>200</em>:</p>

<pre>[
&nbsp; {
&nbsp; &nbsp; "id":2707150273,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":1233932,
&nbsp; &nbsp; &nbsp; "login":"arielchapman",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/1233932"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":481585,
&nbsp; &nbsp; &nbsp; "name":"brianramos/quam-unde-illo",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/brianramos/quam-unde-illo"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2014-07-11 15:13:31"
&nbsp; }
]</pre>
</div>
</details>

<details><summary class="section-title">PUT <code>/actors</code></summary>

<div class="collapsable-details">
<p>The request is sent with the following body. Response should be an empty body with a status code of <em>200</em></p>

<pre>{
&nbsp; "id":2132248,
&nbsp; "login":"robert02",
&nbsp; "avatar_url":"https://avatars.com/modified1"
}</pre>
</div>
</details>

<details><summary class="section-title">GET <code>/events</code></summary>

<div class="collapsable-details">
<p>The response of the <em>GET</em> request is the following <em>JSON</em> array with the <em>HTTP</em> response code <em>200</em>:</p>

<pre>[
&nbsp; {
&nbsp; &nbsp; "id":1351371245,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":1880228,
&nbsp; &nbsp; &nbsp; "login":"joshua15",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/1880228"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":442361,
&nbsp; &nbsp; &nbsp; "name":"joshua15/maiores-aspernatur",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/joshua15/maiores-aspernatur"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2013-04-26 11:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":1706531305,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":2559288,
&nbsp; &nbsp; &nbsp; "login":"upratt",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/2559288"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":369757,
&nbsp; &nbsp; &nbsp; "name":"upratt/maxime-cum-optio-a",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/upratt/maxime-cum-optio-a"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2013-08-17 11:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":1724643219,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":2659286,
&nbsp; &nbsp; &nbsp; "login":"larry92",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/2659286"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":198663,
&nbsp; &nbsp; &nbsp; "name":"larry92/dignissimos",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/larry92/dignissimos"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2013-08-24 00:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":2226511299,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":1834821,
&nbsp; &nbsp; &nbsp; "login":"carrie89",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/1834821"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":332247,
&nbsp; &nbsp; &nbsp; "name":"carrie89/quod-maxime-dolorum",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/carrie89/quod-maxime-dolorum"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2014-02-05 11:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":2707150273,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":1233932,
&nbsp; &nbsp; &nbsp; "login":"arielchapman",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/1233932"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":481585,
&nbsp; &nbsp; &nbsp; "name":"brianramos/quam-unde-illo",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/brianramos/quam-unde-illo"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2014-07-11 15:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":3077377593,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":4933705,
&nbsp; &nbsp; &nbsp; "login":"davistravis",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/4933705"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":103403,
&nbsp; &nbsp; &nbsp; "name":"ngarcia/pariatur",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/ngarcia/pariatur"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2014-11-13 22:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":3541994625,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":2132248,
&nbsp; &nbsp; &nbsp; "login":"robert02",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/modified1"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":293914,
&nbsp; &nbsp; &nbsp; "name":"thomasjones/dolorem-architecto",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/thomasjones/dolorem-architecto"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2015-04-07 19:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":3587954242,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":3271833,
&nbsp; &nbsp; &nbsp; "login":"philip55",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/3271833"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":322322,
&nbsp; &nbsp; &nbsp; "name":"philip55/architecto",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/philip55/architecto"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2015-04-25 18:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":3761013629,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":2301944,
&nbsp; &nbsp; &nbsp; "login":"williamssue",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/2301944"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":363748,
&nbsp; &nbsp; &nbsp; "name":"michael73/maxime-nisi-hic",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/michael73/maxime-nisi-hic"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2015-06-25 09:13:31"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":4803136235,
&nbsp; &nbsp; "type":"PushEvent",
&nbsp; &nbsp; "actor":{
&nbsp; &nbsp; &nbsp; "id":4108139,
&nbsp; &nbsp; &nbsp; "login":"fcoleman",
&nbsp; &nbsp; &nbsp; "avatar_url":"https://avatars.com/4108139"
&nbsp; &nbsp; },
&nbsp; &nbsp; "repo":{
&nbsp; &nbsp; &nbsp; "id":462411,
&nbsp; &nbsp; &nbsp; "name":"yfrazier/sit-fuga-aut-earum",
&nbsp; &nbsp; &nbsp; "url":"https://github.com/yfrazier/sit-fuga-aut-earum"
&nbsp; &nbsp; },
&nbsp; &nbsp; "created_at":"2016-07-02 22:13:31"
&nbsp; }
]</pre>
</div>
</details>

<details><summary class="section-title">GET <code>/actors</code></summary>

<div class="collapsable-details">
<p>The response of the <em>GET</em> request is the following <em>JSON</em> array with the <em>HTTP</em> response code <em>200</em>:</p>

<pre>[
&nbsp; {
&nbsp; &nbsp; "id":4108139,
&nbsp; &nbsp; "login":"fcoleman",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/4108139"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":2301944,
&nbsp; &nbsp; "login":"williamssue",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2301944"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":3271833,
&nbsp; &nbsp; "login":"philip55",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/3271833"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":2132248,
&nbsp; &nbsp; "login":"robert02",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/modified1"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":4933705,
&nbsp; &nbsp; "login":"davistravis",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/4933705"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":1233932,
&nbsp; &nbsp; "login":"arielchapman",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/1233932"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":1834821,
&nbsp; &nbsp; "login":"carrie89",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/1834821"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":2659286,
&nbsp; &nbsp; "login":"larry92",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2659286"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":2559288,
&nbsp; &nbsp; "login":"upratt",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/2559288"
&nbsp; },
&nbsp; {
&nbsp; &nbsp; "id":1880228,
&nbsp; &nbsp; "login":"joshua15",
&nbsp; &nbsp; "avatar_url":"https://avatars.com/1880228"
&nbsp; }
]</pre>

<p>&nbsp;</p>
</div>
</details>

<details><summary class="section-title">DELETE <code>/erase</code></summary>

<div class="collapsable-details">
<p>This request deletes all events and returns an empty body in the response with status code as <em>200</em>.</p>
</div>
</details>
</div>
</details>
</div>
</div>
      <div class="clear"></div>
      <div class="soft-divider mlB"></div>
      
      <div class="qcontent fadeinContent" style="min-height:200px;"><div class="question-project" style="width: 100%;">
<div class="banner mlB csx-tour-banner">
    <div class="js-closetour csx-closetour-button"><a class="btn btn-link">✖</a></div>
    <div class="row csx-tour-row">
        <div class="span15 mmT" style="text-align:left"> We recommend you take a quick tour of our editor before you proceed. The timer will pause up to 90 seconds for the tour. &nbsp; <a class="js-tour btn btn-small btn-primary">Start tour</a></div>
    </div>
</div>
<div id="ck-container" class="candidate">
  <div id="ck" class="codekit-editor cb-smallscreen">
<div id="codekit" class="mode-body-fullpage">
	<!-- Alerts -->
	<div class="cb-alerts"></div>

	<!-- Menu bar -->
	<div class="cb-menubar">
		<div class="lateral-commands cb-commands"><ul class="cb-commands-toolbar"><li class="menu-item ignore"><a href="#" title="" data-original-title="Run">
    <i class="fa fa-play"></i>
</a>
</li><li class="menu-item "><a href="#" title="" data-original-title="Auto Restart On">
    <i class="fa fa-refresh"></i>
</a>
</li><li class="menu-item "><a href="#" title="" data-original-title="New Terminal">
    <i class="fa fa-terminal"></i>
</a>
</li><li class="menu-item "><a href="#" title="" data-original-title="Command Palette">
    <i class="fa fa-bars"></i>
</a>
</li><li class="menu-item "><a href="#" title="" data-original-title="Full Screen Mode">
    <i class="fa fa-arrows-alt"></i>
</a>
</li><li class="menu-item " style="margin-top: 9px;"><span class="txt-white git-label" style="font-size: 14px;">Use Git</span><input id="git-toggle" type="checkbox" style="display: none;"><span class="switchery" style="box-shadow: rgb(194, 199, 208) 0px 0px 0px 0px inset; border-color: rgb(194, 199, 208); transition: border 0.4s, box-shadow 0.4s;" id="git-toggle"><small style="left: 0px; transition: left 0.2s;"></small></span></li></ul></div>
	<div class="cb-commands-menubar"><div class="btn-group menu-command-item"><button class="btn dropdown-toggle" data-toggle="dropdown">File</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="files.file.new"><i class="menu-icon fa fa-sign-blank"></i>New File<span class="menu-label">⎇ ⇧ N</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="files.folder.create"><i class="menu-icon fa fa-sign-blank"></i>New Folder<span class="menu-label">⎇ ⇧ F</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="files.folder.createTerminal"><i class="menu-icon fa fa-sign-blank"></i>New Terminal<span class="menu-label">⎇ ⇧ T</span></a></li><li class="menu-item  menu-item-menu dropdown-submenu"><a href="#" testid="command282" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Open Recent</a></li><li class="menu-item  menu-item-divider divider"></li><li class="menu-item  menu-item-action"><a href="#" testid="refresh.file.tree"><i class="menu-icon fa fa-sign-blank"></i>Refresh File Tree</a></li><li class="menu-item  menu-item-divider divider"></li><li class="menu-item menu-item-red menu-item-action"><a href="#" testid="reset.to.base"><i class="menu-icon fa fa-sign-blank"></i>Reset Project</a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command9034"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command9038"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command9608"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command9612"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command10177"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command10181"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command10750"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command10754"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command11327"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command11331"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command12045"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command12049"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command12756"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command12760"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command13349"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command13353"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item  hidden"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command13943"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command13947"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item"><button class="btn dropdown-toggle" data-toggle="dropdown">Edit</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="command14543"><i class="menu-icon fa fa-sign-blank"></i>Save File<span class="menu-label">⌃ S</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="command14547"><i class="menu-icon fa fa-sign-blank"></i>Close File<span class="menu-label">⎇ W</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item"><button class="btn dropdown-toggle" data-toggle="dropdown">View</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="full.screen"><i class="menu-icon fa fa-sign-blank"></i>Full Screen Mode</a></li><li class="menu-item  menu-item-menu dropdown-submenu"><a href="#" testid="command58" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Layout</a><ul class="dropdown-menu ui-menu"><li class="menu-item  active menu-item-action"><a href="#" testid="command62"><i class="menu-icon fa fa-check"></i>Auto Grid</a></li><li class="menu-item  menu-item-action"><a href="#" testid="command66"><i class="menu-icon fa fa-sign-blank"></i>Columns: 1</a></li><li class="menu-item  menu-item-action"><a href="#" testid="command70"><i class="menu-icon fa fa-sign-blank"></i>Columns: 2</a></li><li class="menu-item  menu-item-action"><a href="#" testid="command74"><i class="menu-icon fa fa-sign-blank"></i>Columns: 3</a></li><li class="menu-item  menu-item-action"><a href="#" testid="command78"><i class="menu-icon fa fa-sign-blank"></i>Columns: 4</a></li></ul></li><li class="menu-item  menu-item-divider divider"></li><li class="menu-item  menu-item-action"><a href="#" testid="settings"><i class="menu-icon fa fa-sign-blank"></i>Settings</a></li></ul></div><div class="btn-group menu-command-item"><button class="btn dropdown-toggle" data-toggle="dropdown">Find</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="code.search"><i class="menu-icon fa fa-sign-blank"></i>Find in Files<span class="menu-label">⌃ ⇧ F</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="code.replace"><i class="menu-icon fa fa-sign-blank"></i>Replace in Files</a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item"><button class="btn dropdown-toggle" data-toggle="dropdown">Run</button><ul class="dropdown-menu ui-menu"><li class="menu-item  menu-item-action"><a href="#" testid="codekit:run"><i class="menu-icon fa fa-sign-blank"></i>Run server<span class="menu-label">⎇ ⇧ R</span></a></li><li class="menu-item  menu-item-action"><a href="#" testid="codekit:install"><i class="menu-icon fa fa-sign-blank"></i>Install</a></li><li class="menu-item  menu-item-action"><a href="#" testid="codekit:test"><i class="menu-icon fa fa-sign-blank"></i>Test</a></li><li class="menu-item  menu-item-divider divider"></li><li class="menu-item  menu-item-action"><a href="#" testid="project.preview.app.menu"><i class="menu-icon fa fa-sign-blank"></i>Preview App<span class="menu-label">⎇ ⇧ V</span></a></li><li class="menu-item  menu-item-divider divider"></li></ul></div><div class="btn-group menu-command-item hidden"><button class="btn btn-no-dropdown"><i class="fa fa-eye mmR"></i>Preview App</button><ul class="dropdown-menu ui-menu"></ul></div><div class="btn-group menu-command-item timer"><button class="btn btn-no-dropdown"><i class="fa fa-clock-o msR"></i>48m</button><ul class="dropdown-menu ui-menu"></ul></div></div></div>

	<!-- Lateral bar commands-->
<!-- 	<div class="cb-lateralbar">
		<div class="lateral-commands cb-commands"></div>
	</div> -->

	<!-- Body -->
	<div class="cb-body with-panel-left"><div class="panel-buttons-container panel-left"><button class="panel-button btn active">File Tree</button><button class="panel-button btn hidden">Question</button></div><div class="component-grid"><div class="grid-section" style="left: 0%; top: 0%; width: 28.45%; height: 100%;"><div class="grid-section-content with-bar-h"><div><div class="cb-panels"><div class="cb-tabs"><div class="component-grid"><div class="grid-section" style="left: 0%; top: 0%; width: 100%; height: 100%;"><div class="grid-section-content"><div class="tabs-section"><ul id="tab-h-scroll" class="hidden"><i class="fa fa-chevron-left tab-h-scroll scroll-left txt-alt-grey-dark"></i><i class="fa fa-chevron-right tab-h-scroll scroll-right txt-alt-grey-dark"></i></ul><ul class="tabs-section-header"><li class="component-tab active"><div class="inner"><a class="close" href="javascript:void(0);">×</a>Project</div></li></ul><ul class="tabs-section-content"><li class="component-tab-content active"><div class="component-tab-panel"><div class="cb-panel-files"><ul class="root-tree cb-files-tree"><li class="file-item open type-directory"><span class="name " style="padding-left: 8px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder-o file-icon"></i>
      <i class="fa fa-folder-open-o file-icon"></i>
      
    
    project
</span>

    <div class="files"><ul class="cb-files-tree root"><li class="file-item type-directory open"><span class="name " style="padding-left: 31px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    src
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 54px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    main
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 77px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    java
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 100px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    com
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    hackerrank
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 146px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    github
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 169px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    controller
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item"><span class="name " style="padding-left: 192px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    GithubApiRestController.java
</span>

</li></ul></div>

</li><li class="file-item type-directory open"><span class="name " style="padding-left: 169px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    model
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item"><span class="name " style="padding-left: 192px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    Actor.java
</span>

</li><li class="file-item"><span class="name " style="padding-left: 192px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    Event.java
</span>

</li><li class="file-item"><span class="name " style="padding-left: 192px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    Repo.java
</span>

</li></ul></div>

</li><li class="file-item type-directory open"><span class="name " style="padding-left: 169px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    repository
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item"><span class="name " style="padding-left: 192px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    ActorRepository.java
</span>

</li><li class="file-item"><span class="name " style="padding-left: 192px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    EventRepository.java
</span>

</li><li class="file-item"><span class="name " style="padding-left: 192px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    RepoRepository.java
</span>

</li></ul></div>

</li><li class="file-item active"><span class="name " style="padding-left: 169px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    Application.java
</span>

</li></ul></div>

</li></ul></div>

</li></ul></div>

</li></ul></div>

</li><li class="file-item type-directory open"><span class="name " style="padding-left: 77px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    resources
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item"><span class="name " style="padding-left: 100px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    application.properties
</span>

</li></ul></div>

</li></ul></div>

</li><li class="file-item type-directory open"><span class="name " style="padding-left: 54px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    test
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 77px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    java
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 100px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    com
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    hackerrank
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 146px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    github
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item"><span class="name " style="padding-left: 169px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    HttpJsonDynamicUnitTest.java
</span>

</li></ul></div>

</li></ul></div>

</li></ul></div>

</li></ul></div>

</li><li class="file-item type-directory open"><span class="name " style="padding-left: 77px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    resources
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory open"><span class="name " style="padding-left: 100px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    testcases
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    description.txt
</span>

</li><li class="file-item"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    http00.json
</span>

</li><li class="file-item"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    http01.json
</span>

</li><li class="file-item"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    http02.json
</span>

</li><li class="file-item"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    http03.json
</span>

</li><li class="file-item"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    http04.json
</span>

</li><li class="file-item"><span class="name " style="padding-left: 123px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    http05.json
</span>

</li></ul></div>

</li></ul></div>

</li></ul></div>

</li></ul></div>

</li><li class="file-item type-directory"><span class="name " style="padding-left: 31px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    target
</span>

    <div class="files"><ul class="cb-files-tree"><li class="file-item type-directory"><span class="name " style="padding-left: 54px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    classes
</span>

    <div class="files"></div>

</li><li class="file-item type-directory"><span class="name " style="padding-left: 54px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    generated-sources
</span>

    <div class="files"></div>

</li><li class="file-item type-directory"><span class="name " style="padding-left: 54px;">
    
    <i class="fa fa-angle-right"></i>
    <i class="fa fa-angle-down"></i>
    <i class="fa fa-hourglass-half"></i>
      
      <i class="fa fa-folder file-icon"></i>
      <i class="fa fa-folder-open file-icon"></i>
      
    
    maven-status
</span>

    <div class="files"></div>

</li></ul></div>

</li><li class="file-item"><span class="name " style="padding-left: 31px;">
    
    <i class="fa fa-angle-right invisible"></i>
    <i class="fa fa-file-text-o file-icon"></i>
    
    pom.xml
</span>

</li></ul></div>

</li></ul></div></div></li></ul></div></div></div></div></div></div><ul class="cb-operations"><div class="hr-list-message hr-list-message-empty"></div></ul></div></div><div class="grid-resize-bar-h"></div></div><div class="grid-section" style="left: 28.45%; top: 0%; width: 71.55%; height: 100%;"><div class="grid-section-content with-bar-h"><div class="cb-tabs"><div class="component-grid"><div class="grid-section" style="left: 0%; top: 0%; width: 100%; height: 100%;"><div class="grid-section-content"><div class="tabs-section"><ul id="tab-h-scroll" class=""><i class="fa fa-chevron-left tab-h-scroll scroll-left txt-alt-grey-dark"></i><i class="fa fa-chevron-right tab-h-scroll scroll-right txt-alt-grey-dark"></i></ul><ul class="tabs-section-header" style="margin-left: -1167.56px;"><li class="component-tab" style="left: auto; top: auto;"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>Actor.java</div></li><li class="component-tab" style="left: auto; top: auto;"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>GithubApiRestController.java</div></li><li class="component-tab" style="left: auto; top: auto;"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>http00.json</div></li><li class="component-tab" style="left: auto; top: auto;"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>Event.java</div></li><li class="component-tab" style="left: auto; top: auto;"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>Repo.java</div></li><li class="component-tab"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>pom.xml</div></li><li class="component-tab"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>ActorRepository.java</div></li><li class="component-tab"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>EventRepository.java</div></li><li class="component-tab"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>RepoRepository.java</div></li><li class="component-tab active"><div class="inner"><a class="close" href="javascript:void(0);">×</a><i class="state fa fa-file-text-o"></i>Application.java</div></li></ul><ul class="tabs-section-content"><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;" draggable="false"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 51px; top: 560px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 47px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div><div class="ace_gutter-cell " style="height: 14px;">6</div><div class="ace_gutter-cell " style="height: 14px;">7</div><div class="ace_gutter-cell " style="height: 14px;">8<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">9</div><div class="ace_gutter-cell " style="height: 14px;">10</div><div class="ace_gutter-cell " style="height: 14px;">11<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">12</div><div class="ace_gutter-cell " style="height: 14px;">13</div><div class="ace_gutter-cell " style="height: 14px;">14</div><div class="ace_gutter-cell " style="height: 14px;">15</div><div class="ace_gutter-cell " style="height: 14px;">16</div><div class="ace_gutter-cell " style="height: 14px;">17<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">18</div><div class="ace_gutter-cell " style="height: 14px;">19</div><div class="ace_gutter-cell " style="height: 14px;">20</div><div class="ace_gutter-cell " style="height: 14px;">21<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">22</div><div class="ace_gutter-cell " style="height: 14px;">23</div><div class="ace_gutter-cell " style="height: 14px;">24</div><div class="ace_gutter-cell " style="height: 14px;">25<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">26</div><div class="ace_gutter-cell " style="height: 14px;">27</div><div class="ace_gutter-cell " style="height: 14px;">28</div><div class="ace_gutter-cell " style="height: 14px;">29<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">30</div><div class="ace_gutter-cell " style="height: 14px;">31</div><div class="ace_gutter-cell " style="height: 14px;">32</div><div class="ace_gutter-cell " style="height: 14px;">33<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">34</div><div class="ace_gutter-cell " style="height: 14px;">35</div><div class="ace_gutter-cell " style="height: 14px;">36</div><div class="ace_gutter-cell " style="height: 14px;">37<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">38</div><div class="ace_gutter-cell " style="height: 14px;">39</div><div class="ace_gutter-cell " style="height: 14px;">40</div><div class="ace_gutter-cell " style="height: 14px;">41</div></div><div class="ace_gutter-active-line" style="top: 560px; height: 14px;"></div></div><div class="ace_scroller" style="left: 47px; right: 0px; bottom: 0px;"><div class="ace_content" style="margin-top: 0px; width: 1124px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:28px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:560px;left:4px;"></div><div class="ace_selection ace_br8" style="height:518px;right:0;top:42px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>.<span class="ace_identifier">model</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">class</span> <span class="ace_identifier">Actor</span> {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">login</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">avatar</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_identifier">Actor</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_identifier">Actor</span>(<span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>, <span class="ace_support ace_function">String</span> <span class="ace_identifier">login</span>, <span class="ace_support ace_function">String</span> <span class="ace_identifier">avatar</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">id</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">login</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">login</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">avatar</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">avatar</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    </div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">Long</span> <span class="ace_identifier">getId</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    </div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setId</span>(<span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">id</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    </div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">getLogin</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">login</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    </div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setLogin</span>(<span class="ace_support ace_function">String</span> <span class="ace_identifier">login</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">login</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">login</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    </div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">getAvatar</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">avatar</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    </div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setAvatar</span>(<span class="ace_support ace_function">String</span> <span class="ace_identifier">avatar</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">avatar</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">avatar</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">}</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 560px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="width: 20px; bottom: 0px; display: none;"><div class="ace_scrollbar-inner" style="width: 20px; height: 574px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 47px; right: 0px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 1124px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 44px; top: 42px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 40px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3</div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div><div class="ace_gutter-cell " style="height: 14px;">6<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">7</div><div class="ace_gutter-cell " style="height: 14px;">8</div></div><div class="ace_gutter-active-line" style="top: 42px; height: 14px;"></div></div><div class="ace_scroller" style="left: 40px; right: 0px; bottom: 0px;"><div class="ace_content" style="margin-top: 0px; width: 1131px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:28px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:42px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>.<span class="ace_identifier">controller</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">import</span> <span class="ace_identifier">org</span>.<span class="ace_identifier">springframework</span>.<span class="ace_identifier">web</span>.<span class="ace_identifier">bind</span>.<span class="ace_identifier">annotation</span>.<span class="ace_identifier">RestController</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">@<span class="ace_identifier">RestController</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">class</span> <span class="ace_identifier">GithubApiRestController</span> {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">}</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 42px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="display: none; width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 112px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 40px; right: 0px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 1131px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;" draggable="false"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; left: 0px; top: 0px; height: 14px; width: 7px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 714px; width: 47px;"><div class="ace_gutter-cell  ace_error" style="height: 56px;">1</div><div class="ace_gutter-cell " style="height: 56px;">2</div><div class="ace_gutter-cell " style="height: 56px;">3</div><div class="ace_gutter-cell " style="height: 56px;">4</div><div class="ace_gutter-cell " style="height: 56px;">5</div><div class="ace_gutter-cell " style="height: 56px;">6</div><div class="ace_gutter-cell " style="height: 56px;">7</div><div class="ace_gutter-cell " style="height: 56px;">8</div><div class="ace_gutter-cell " style="height: 56px;">9</div><div class="ace_gutter-cell " style="height: 56px;">10</div><div class="ace_gutter-cell " style="height: 56px;">11</div></div><div class="ace_gutter-active-line" style="top: 1148px; height: 28px;"></div></div><div class="ace_scroller" style="left: 47px; right: 15px; bottom: 0px; cursor: default;"><div class="ace_content" style="margin-top: 0px; width: 923px; height: 714px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:0px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:616px;left:4px;"></div><div class="ace_selection ace_br8" style="height:602px;right:0;top:14px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">3761013629</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">2301944</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"williamssue"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/2301944"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">363748</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"michael73/maxime-nisi-hic"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/michael73/maxime-nisi-hic"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">"2015-06-25 09:13:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">2226511299</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">1834821</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"carrie89"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/1834821"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;: <span class="ace_constant ace_numeric">332247</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"carrie89/quod-maxime-dolorum"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/carrie89/quod-maxime-dolorum"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">"2014-02-05 11:13:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">3077377593</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">4933705</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"davistravis"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/4933705"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">103403</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"ngarcia/pariatur"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/ngarcia/pariatur"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: <span class="ace_string">"2014-11-13 22:13</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">1706531305</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">2559288</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"upratt"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/2559288"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_constant ace_numeric">369757</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"upratt/maxime-cum-optio-a"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/upratt/maxime-cum-optio-a"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: <span class="ace_string">"2013-08-17 </span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">11:13:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">1351371245</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">1880228</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"joshua15"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/1880228"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;: <span class="ace_constant ace_numeric">442361</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"joshua15/maiores-aspernatur"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/joshua15/maiores-aspernatur"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: <span class="ace_string">"2013</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">-04-26 11:13:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">3541994625</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">2132248</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"robert02"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/2132248"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;: <span class="ace_constant ace_numeric">293914</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"thomasjones/dolorem-architecto"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/thomasjones/dolorem-architecto"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">"2015-04-07 19:13:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">4803136235</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">4108139</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"fcoleman"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/4108139"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;: <span class="ace_constant ace_numeric">462411</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"yfrazier/sit-fuga-aut-earum"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/yfrazier/sit-fuga-aut-earum"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: <span class="ace_string">"2016</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">-07-02 22:13:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">3587954242</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">3271833</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"philip55"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/3271833"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;: <span class="ace_constant ace_numeric">322322</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"philip55/architecto"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/philip55/architecto"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: <span class="ace_string">"2015-04-25 18:13</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">1724643219</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">2659286</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"larry92"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/2659286"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_constant ace_numeric">198663</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"larry92/dignissimos"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/larry92/dignissimos"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: <span class="ace_string">"2013-08-24 00:13:31"</span><span class="ace_paren ace_rparen">}}</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"POST"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">2707150273</span>, </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">1233932</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"arielchapman"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars.com/1233932"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">481585</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"brianramos/quam-unde-illo"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/brianramos/quam-unde-illo"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: </div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">"2014-07-11 15:13:31"</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">201</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}}</span></div></div><div class="ace_line_group" style="height:56px"><div class="ace_line" style="height:14px"><span class="ace_paren ace_lparen">{</span><span class="ace_variable">"request"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"method"</span>: <span class="ace_string">"GET"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"/events/actors/1233932"</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"body"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_paren ace_rparen">}}</span>, <span class="ace_variable">"response"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"status_code"</span>: <span class="ace_constant ace_numeric">200</span>, <span class="ace_variable">"body"</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;: <span class="ace_paren ace_lparen">[{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">2707150273</span>, <span class="ace_variable">"type"</span>: <span class="ace_string">"PushEvent"</span>, <span class="ace_variable">"actor"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">1233932</span>, <span class="ace_variable">"login"</span>: <span class="ace_string">"arielchapman"</span>, <span class="ace_variable">"avatar_url"</span>: <span class="ace_string">"https://avatars</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">.com/1233932"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"repo"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"id"</span>: <span class="ace_constant ace_numeric">481585</span>, <span class="ace_variable">"name"</span>: <span class="ace_string">"brianramos/quam-unde-illo"</span>, <span class="ace_variable">"url"</span>: <span class="ace_string">"https://github.com/brianramos/quam-unde</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string">-illo"</span><span class="ace_paren ace_rparen">}</span>, <span class="ace_variable">"created_at"</span>: <span class="ace_string">"2014-07-11 15:13:31"</span><span class="ace_paren ace_rparen">}]</span>, <span class="ace_variable">"headers"</span>: <span class="ace_paren ace_lparen">{</span><span class="ace_variable">"Content-Type"</span>: <span class="ace_string">"application/json"</span><span class="ace_paren ace_rparen">}}}</span></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 312px; top: 1162px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 1176px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 47px; right: 15px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 923px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div><div class="ace_tooltip" style="display: none; left: 377px; top: 484px;">Parse error on line 1:
...{}, "headers": {}}}{"request": {"method
----------------------^
Expecting 'EOF', '}', ',', ']', got '{'</div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 0px; top: 0px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 47px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3</div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">6</div><div class="ace_gutter-cell " style="height: 14px;">7</div><div class="ace_gutter-cell " style="height: 14px;">8</div><div class="ace_gutter-cell " style="height: 14px;">9</div><div class="ace_gutter-cell " style="height: 14px;">10</div><div class="ace_gutter-cell " style="height: 14px;">11</div><div class="ace_gutter-cell " style="height: 14px;">12<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">13</div><div class="ace_gutter-cell " style="height: 14px;">14</div><div class="ace_gutter-cell " style="height: 14px;">15<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">16</div><div class="ace_gutter-cell " style="height: 14px;">17</div><div class="ace_gutter-cell " style="height: 14px;">18</div><div class="ace_gutter-cell " style="height: 14px;">19</div><div class="ace_gutter-cell " style="height: 14px;">20</div><div class="ace_gutter-cell " style="height: 14px;">21</div><div class="ace_gutter-cell " style="height: 14px;">22</div><div class="ace_gutter-cell " style="height: 14px;">23<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">24</div><div class="ace_gutter-cell " style="height: 14px;">25</div><div class="ace_gutter-cell " style="height: 14px;">26</div><div class="ace_gutter-cell " style="height: 14px;">27<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">28</div><div class="ace_gutter-cell " style="height: 14px;">29</div><div class="ace_gutter-cell " style="height: 14px;">30</div><div class="ace_gutter-cell " style="height: 14px;">31<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">32</div><div class="ace_gutter-cell " style="height: 14px;">33</div><div class="ace_gutter-cell " style="height: 14px;">34</div><div class="ace_gutter-cell " style="height: 14px;">35<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">36</div><div class="ace_gutter-cell " style="height: 14px;">37</div><div class="ace_gutter-cell " style="height: 14px;">38</div><div class="ace_gutter-cell " style="height: 14px;">39<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">40</div><div class="ace_gutter-cell " style="height: 14px;">41</div><div class="ace_gutter-cell " style="height: 14px;">42</div><div class="ace_gutter-cell " style="height: 14px;">43<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">44</div></div><div class="ace_gutter-active-line" style="top: 868px; height: 14px;"></div></div><div class="ace_scroller" style="left: 47px; right: 15px; bottom: 0px; cursor: default;"><div class="ace_content" style="margin-top: 0px; width: 1109px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:0px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:616px;left:4px;"></div><div class="ace_selection ace_br8" style="height:602px;right:0;top:14px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>.<span class="ace_identifier">model</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_keyword">import</span> <span class="ace_identifier">java</span>.<span class="ace_identifier">sql</span>.<span class="ace_identifier">Timestamp</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">class</span> <span class="ace_identifier">Event</span> {</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">type</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_identifier">Actor</span> <span class="ace_identifier">actor</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_identifier">Repo</span> <span class="ace_identifier">repo</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_identifier">Timestamp</span> <span class="ace_identifier">createdAt</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_identifier">Event</span>() {</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_identifier">Event</span>(<span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>, <span class="ace_support ace_function">String</span> <span class="ace_identifier">type</span>, <span class="ace_identifier">Actor</span> <span class="ace_identifier">actor</span>, <span class="ace_identifier">Repo</span> <span class="ace_identifier">repo</span>, <span class="ace_identifier">Timestamp</span> <span class="ace_identifier">createdAt</span>) {</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">id</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">type</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">type</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">actor</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">actor</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">repo</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">repo</span>;</div></div><div class="ace_line_group" style="height: 14px;"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">createdAt</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">createdAt</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">Long</span> <span class="ace_identifier">getId</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setId</span>(<span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">id</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">getType</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">type</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setType</span>(<span class="ace_support ace_function">String</span> <span class="ace_identifier">type</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">type</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">type</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_identifier">Actor</span> <span class="ace_identifier">getActor</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">actor</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setActor</span>(<span class="ace_identifier">Actor</span> <span class="ace_identifier">actor</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">actor</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">actor</span>;</div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 868px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 882px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 47px; right: 15px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 1109px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;" draggable="false"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 86px; top: 252px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 47px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div><div class="ace_gutter-cell " style="height: 14px;">6</div><div class="ace_gutter-cell " style="height: 14px;">7</div><div class="ace_gutter-cell " style="height: 14px;">8<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">9</div><div class="ace_gutter-cell " style="height: 14px;">10</div><div class="ace_gutter-cell " style="height: 14px;">11<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">12</div><div class="ace_gutter-cell " style="height: 14px;">13</div><div class="ace_gutter-cell " style="height: 14px;">14</div><div class="ace_gutter-cell " style="height: 14px;">15</div><div class="ace_gutter-cell " style="height: 14px;">16</div><div class="ace_gutter-cell " style="height: 14px;">17<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">18</div><div class="ace_gutter-cell " style="height: 14px;">19</div><div class="ace_gutter-cell " style="height: 14px;">20</div><div class="ace_gutter-cell " style="height: 14px;">21<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">22</div><div class="ace_gutter-cell " style="height: 14px;">23</div><div class="ace_gutter-cell " style="height: 14px;">24</div><div class="ace_gutter-cell " style="height: 14px;">25<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">26</div><div class="ace_gutter-cell " style="height: 14px;">27</div><div class="ace_gutter-cell " style="height: 14px;">28</div><div class="ace_gutter-cell " style="height: 14px;">29<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">30</div><div class="ace_gutter-cell " style="height: 14px;">31</div><div class="ace_gutter-cell " style="height: 14px;">32</div><div class="ace_gutter-cell " style="height: 14px;">33<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">34</div><div class="ace_gutter-cell " style="height: 14px;">35</div><div class="ace_gutter-cell " style="height: 14px;">36</div><div class="ace_gutter-cell " style="height: 14px;">37<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">38</div><div class="ace_gutter-cell " style="height: 14px;">39</div><div class="ace_gutter-cell " style="height: 14px;">40</div><div class="ace_gutter-cell " style="height: 14px;">41</div></div><div class="ace_gutter-active-line" style="top: 252px; height: 14px;"></div></div><div class="ace_scroller" style="left: 47px; right: 0px; bottom: 0px;"><div class="ace_content" style="margin-top: 0px; width: 1124px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_bracket ace_start ace_br15" style="height:14px;width:7px;top:224px;left:172px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>.<span class="ace_identifier">model</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">class</span> <span class="ace_identifier">Repo</span> {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">name</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">url</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_identifier">Repo</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_identifier">Repo</span>(<span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>, <span class="ace_support ace_function">String</span> <span class="ace_identifier">name</span>, <span class="ace_support ace_function">String</span> <span class="ace_identifier">url</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">id</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">name</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">name</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">url</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">url</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">Long</span> <span class="ace_identifier">getId</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setId</span>(<span class="ace_support ace_function">Long</span> <span class="ace_identifier">id</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">id</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">id</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">getName</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">name</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setName</span>(<span class="ace_support ace_function">String</span> <span class="ace_identifier">name</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">name</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">name</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_support ace_function">String</span> <span class="ace_identifier">getUrl</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">return</span> <span class="ace_identifier">url</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setUrl</span>(<span class="ace_support ace_function">String</span> <span class="ace_identifier">url</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_keyword">this</span>.<span class="ace_identifier">url</span> <span class="ace_keyword ace_operator">=</span> <span class="ace_identifier">url</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">}</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 39px; top: 252px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="display: none; width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 574px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 47px; right: 0px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 1124px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 0px; top: 0px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 47px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 28px;">2<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">3</div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div><div class="ace_gutter-cell " style="height: 14px;">6</div><div class="ace_gutter-cell " style="height: 14px;">7</div><div class="ace_gutter-cell " style="height: 14px;">8</div><div class="ace_gutter-cell " style="height: 14px;">9</div><div class="ace_gutter-cell " style="height: 14px;">10<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">11</div><div class="ace_gutter-cell " style="height: 14px;">12</div><div class="ace_gutter-cell " style="height: 14px;">13</div><div class="ace_gutter-cell " style="height: 14px;">14</div><div class="ace_gutter-cell " style="height: 14px;">15</div><div class="ace_gutter-cell " style="height: 14px;">16<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">17</div><div class="ace_gutter-cell " style="height: 14px;">18</div><div class="ace_gutter-cell " style="height: 14px;">19</div><div class="ace_gutter-cell " style="height: 14px;">20</div><div class="ace_gutter-cell " style="height: 14px;">21</div><div class="ace_gutter-cell " style="height: 14px;">22</div><div class="ace_gutter-cell " style="height: 14px;">23<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">24<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">25</div><div class="ace_gutter-cell " style="height: 14px;">26</div><div class="ace_gutter-cell " style="height: 14px;">27</div><div class="ace_gutter-cell " style="height: 14px;">28</div><div class="ace_gutter-cell " style="height: 14px;">29<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">30</div><div class="ace_gutter-cell " style="height: 14px;">31</div><div class="ace_gutter-cell " style="height: 14px;">32</div><div class="ace_gutter-cell " style="height: 14px;">33</div><div class="ace_gutter-cell " style="height: 14px;">34<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">35</div><div class="ace_gutter-cell " style="height: 14px;">36</div><div class="ace_gutter-cell " style="height: 14px;">37</div><div class="ace_gutter-cell " style="height: 14px;">38</div><div class="ace_gutter-cell " style="height: 14px;">39</div><div class="ace_gutter-cell " style="height: 14px;">40<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">41</div><div class="ace_gutter-cell " style="height: 14px;">42</div><div class="ace_gutter-cell " style="height: 14px;">43</div></div><div class="ace_gutter-active-line" style="top: 882px; height: 14px;"></div></div><div class="ace_scroller" style="left: 47px; right: 15px; bottom: 0px; cursor: default;"><div class="ace_content" style="margin-top: 0px; width: 923px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:0px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:616px;left:4px;"></div><div class="ace_selection ace_br8" style="height:602px;right:0;top:14px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_punctuation ace_instruction ace_xml">&lt;?</span><span class="ace_keyword ace_instruction ace_xml">xml</span><span class="ace_text ace_whitespace ace_xml"> </span><span class="ace_entity ace_other ace_attribute-name ace_decl-attribute-name ace_xml">version</span><span class="ace_keyword ace_operator ace_decl-attribute-equals ace_xml">=</span><span class="ace_string ace_xml">"1.0"</span><span class="ace_text ace_whitespace ace_xml"> </span><span class="ace_entity ace_other ace_attribute-name ace_decl-attribute-name ace_xml">encoding</span><span class="ace_keyword ace_operator ace_decl-attribute-equals ace_xml">=</span><span class="ace_string ace_xml">"UTF-8"</span><span class="ace_punctuation ace_xml-decl ace_xml">?&gt;</span></div></div><div class="ace_line_group" style="height:28px"><div class="ace_line" style="height:14px"><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">project</span><span class="ace_text ace_tag-whitespace ace_xml"> </span><span class="ace_entity ace_other ace_attribute-name ace_xml">xmlns</span><span class="ace_keyword ace_operator ace_attribute-equals ace_xml">=</span><span class="ace_string ace_attribute-value ace_xml">"http://maven.apache.org/POM/4.0.0"</span><span class="ace_text ace_tag-whitespace ace_xml"> </span><span class="ace_entity ace_other ace_attribute-name ace_xml">xmlns:xsi</span><span class="ace_keyword ace_operator ace_attribute-equals ace_xml">=</span><span class="ace_string ace_attribute-value ace_xml">"http://www.w3.org/2001/XMLSchema-instance"</span><span class="ace_text ace_tag-whitespace ace_xml"> </span><span class="ace_entity ace_other ace_attribute-name ace_xml">xsi:schemaLocation</span><span class="ace_keyword ace_operator ace_attribute-equals ace_xml">=</span><span class="ace_string ace_attribute-value ace_xml">"http</span></div><div class="ace_line" style="height:14px">&nbsp;&nbsp;&nbsp;&nbsp;<span class="ace_string ace_attribute-value ace_xml">://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd"</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">modelVersion</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">4.0.0</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">modelVersion</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">com.hackerrank</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">github</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">version</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">1.0-SNAPSHOT</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">version</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">packaging</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">jar</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">packaging</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">properties</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">project.build.sourceEncoding</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">UTF-8</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">project.build.sourceEncoding</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">maven.compiler.source</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">1.8</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">maven.compiler.source</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">maven.compiler.target</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">1.8</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">maven.compiler.target</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">properties</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">parent</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">org.springframework.boot</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">spring-boot-starter-parent</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">version</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">1.5.6.RELEASE</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">version</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">relativePath</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">/&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">parent</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependencies</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependency</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">org.springframework.boot</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">spring-boot-starter-data-jpa</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependency</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependency</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">org.springframework.boot</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">spring-boot-starter-web</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependency</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependency</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">com.h2database</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">h2</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">scope</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">runtime</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">scope</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependency</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">dependency</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">org.springframework.boot</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">groupId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">spring-boot-starter-test</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">artifactId</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_indent-guide">    </span><span class="ace_text ace_xml">    </span><span class="ace_meta ace_tag ace_punctuation ace_tag-open ace_xml">&lt;</span><span class="ace_meta ace_tag ace_tag-name ace_xml">scope</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span><span class="ace_text ace_xml">test</span><span class="ace_meta ace_tag ace_punctuation ace_end-tag-open ace_xml">&lt;/</span><span class="ace_meta ace_tag ace_tag-name ace_xml">scope</span><span class="ace_meta ace_tag ace_punctuation ace_tag-close ace_xml">&gt;</span></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 882px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 896px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 47px; right: 15px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 923px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;" draggable="false"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 44px; top: 56px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 40px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div></div><div class="ace_gutter-active-line" style="top: 56px; height: 14px;"></div></div><div class="ace_scroller" style="left: 40px; right: 0px; bottom: 0px;"><div class="ace_content" style="margin-top: 0px; width: 945px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:0px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:56px;left:4px;"></div><div class="ace_selection ace_br8" style="height:42px;right:0;top:14px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>.<span class="ace_identifier">repository</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">interface</span> <span class="ace_identifier">ActorRepository</span> {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">}</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 56px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="display: none; width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 70px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 40px; right: 0px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 945px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 44px; top: 0px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 40px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div></div><div class="ace_gutter-active-line" style="top: 0px; height: 14px;"></div></div><div class="ace_scroller" style="left: 40px; right: 0px; bottom: 0px;"><div class="ace_content" style="margin-top: 0px; width: 945px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:0px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:56px;left:4px;"></div><div class="ace_selection ace_br8" style="height:42px;right:0;top:14px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>.<span class="ace_identifier">repository</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">interface</span> <span class="ace_identifier">EventRepository</span> {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">}</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 0px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="display: none; width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 70px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 40px; right: 0px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 945px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 44px; top: 0px;" _ar_hide_="width:0px;height:0px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 40px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div></div><div class="ace_gutter-active-line" style="top: 0px; height: 14px;"></div></div><div class="ace_scroller" style="left: 40px; right: 0px; bottom: 0px;"><div class="ace_content" style="margin-top: 0px; width: 945px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:0px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:56px;left:4px;"></div><div class="ace_selection ace_br8" style="height:42px;right:0;top:14px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>.<span class="ace_identifier">repository</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">interface</span> <span class="ace_identifier">RepoRepository</span> {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">}</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 0px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="display: none; width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 70px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 40px; right: 0px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 945px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li><li class="component-tab-content active"><div class="component-tab-panel"><div class="addon-files-aceeditor"><div class="tab-panel-body editor">
    <div class="tab-panel-inner editor-inner"><div class="editor-ace ace_editor ace-dawn" style="font-size: 14px;"><textarea class="ace_text-input _ar_hide_" wrap="off" autocorrect="off" autocapitalize="off" spellcheck="false" style="opacity: 0; height: 14px; width: 7px; left: 51px; top: 0px;" _ar_hide_="width:7px;height:14px;"></textarea><div class="ace_gutter"><div class="ace_layer ace_gutter-layer ace_folding-enabled" style="margin-top: 0px; height: 630px; width: 47px;"><div class="ace_gutter-cell " style="height: 14px;">1</div><div class="ace_gutter-cell " style="height: 14px;">2</div><div class="ace_gutter-cell " style="height: 14px;">3</div><div class="ace_gutter-cell " style="height: 14px;">4</div><div class="ace_gutter-cell " style="height: 14px;">5</div><div class="ace_gutter-cell " style="height: 14px;">6</div><div class="ace_gutter-cell " style="height: 14px;">7</div><div class="ace_gutter-cell " style="height: 14px;">8</div><div class="ace_gutter-cell " style="height: 14px;">9<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">10<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">11</div><div class="ace_gutter-cell " style="height: 14px;">12</div><div class="ace_gutter-cell " style="height: 14px;">13</div><div class="ace_gutter-cell " style="height: 14px;">14</div><div class="ace_gutter-cell " style="height: 14px;">15<span class="ace_fold-widget ace_start ace_open" style="height: 14px;"></span></div><div class="ace_gutter-cell " style="height: 14px;">16</div><div class="ace_gutter-cell " style="height: 14px;">17</div><div class="ace_gutter-cell " style="height: 14px;">18</div><div class="ace_gutter-cell " style="height: 14px;">19</div></div><div class="ace_gutter-active-line" style="top: 0px; height: 14px;"></div></div><div class="ace_scroller" style="left: 47px; right: 0px; bottom: 0px; cursor: default;"><div class="ace_content" style="margin-top: 0px; width: 541px; height: 630px; margin-left: 0px;"><div class="ace_layer ace_print-margin-layer"><div class="ace_print-margin" style="left: 564px; visibility: hidden;"></div></div><div class="ace_layer ace_marker-layer"><div class="ace_selection ace_br1 ace_start" style="height:14px;right:0;top:0px;left:4px;"></div><div class="ace_selection ace_br12" style="height:14px;width:0px;top:252px;left:4px;"></div><div class="ace_selection ace_br8" style="height:238px;right:0;top:14px;left:4px;"></div></div><div class="ace_layer ace_text-layer" style="padding: 0px 4px;"><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">package</span> <span class="ace_identifier">com</span>.<span class="ace_identifier">hackerrank</span>.<span class="ace_identifier">github</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">import</span> <span class="ace_identifier">java</span>.<span class="ace_identifier">util</span>.<span class="ace_identifier">TimeZone</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">import</span> <span class="ace_identifier">javax</span>.<span class="ace_identifier">annotation</span>.<span class="ace_identifier">PostConstruct</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">import</span> <span class="ace_identifier">org</span>.<span class="ace_identifier">springframework</span>.<span class="ace_identifier">boot</span>.<span class="ace_identifier">SpringApplication</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">import</span> <span class="ace_identifier">org</span>.<span class="ace_identifier">springframework</span>.<span class="ace_identifier">boot</span>.<span class="ace_identifier">autoconfigure</span>.<span class="ace_identifier">SpringBootApplication</span>;</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">@<span class="ace_identifier">SpringBootApplication</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_keyword">public</span> <span class="ace_keyword">class</span> <span class="ace_identifier">Application</span> {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">public</span> <span class="ace_keyword">static</span> <span class="ace_keyword">void</span> <span class="ace_identifier">main</span>(<span class="ace_support ace_function">String</span>[] <span class="ace_identifier">args</span>) {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_identifier">SpringApplication</span>.<span class="ace_identifier">run</span>(<span class="ace_identifier">Application</span>.<span class="ace_keyword">class</span>, <span class="ace_identifier">args</span>);</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    </div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    @<span class="ace_identifier">PostConstruct</span></div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    <span class="ace_keyword">private</span> <span class="ace_keyword">void</span> <span class="ace_identifier">setTimeZone</span>() {</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"><span class="ace_indent-guide">    </span>    <span class="ace_identifier">TimeZone</span>.<span class="ace_identifier">setDefault</span>(<span class="ace_identifier">TimeZone</span>.<span class="ace_identifier">getTimeZone</span>(<span class="ace_string">"UTC"</span>));</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">    }</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px">}</div></div><div class="ace_line_group" style="height:14px"><div class="ace_line" style="height:14px"></div></div></div><div class="ace_layer ace_marker-layer"></div><div class="ace_layer ace_cursor-layer ace_hidden-cursors"><div class="ace_cursor" style="left: 4px; top: 0px; width: 7px; height: 14px;"></div></div></div></div><div class="ace_scrollbar ace_scrollbar-v" style="display: none; width: 20px; bottom: 0px;"><div class="ace_scrollbar-inner" style="width: 20px; height: 266px;"></div></div><div class="ace_scrollbar ace_scrollbar-h" style="display: none; height: 20px; left: 47px; right: 0px;"><div class="ace_scrollbar-inner" style="height: 20px; width: 541px;"></div></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: hidden;"><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;"></div><div style="height: auto; width: auto; top: 0px; left: 0px; visibility: hidden; position: absolute; white-space: pre; font-style: inherit; font-variant: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; overflow: visible;">XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX</div></div></div></div>
</div></div></div></li></ul></div></div></div></div></div></div><div class="grid-resize-bar-h"></div></div><div class="grid-section" style="left: 100%; top: 0%; width: 0%; height: 100%;"><div class="grid-section-content"><div><div class="cb-panels"><div class="cb-tabs"><div class="component-grid"></div></div></div></div></div></div></div><div class="cb-commands-palette close"><input type="text" class="form-control palette-input input-sm _ar_hide_" value="" placeholder="Search Files or Enter Command">
<div class="results"><ul class="palette-commands"><div class="hr-list-message hr-list-message-empty"></div></ul></div></div><div class="panel-buttons-container panel-right"><button class="panel-button btn hidden">Preview App</button></div></div>

	<!-- Status bar -->
	<div class="cb-statusbar"><ul class="cb-commands-menubar"><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 41, Column 1</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command8521" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command9009"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 4, Column 1</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command9095" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command9583"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>JSON</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 16, Column 171</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command9664" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command10152"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 63, Column 1</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command10237" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command10725"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 19, Column 6</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command10814" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command11302"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>XML</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 63, Column 1</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command11532" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command12020"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 5, Column 1</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command12243" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command12731"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 1, Column 1</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command12836" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command13324"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  hidden menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 1, Column 1</li><li class="menu-item  hidden menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  hidden menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command13430" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  hidden menu-item-action"><a href="#" testid="command13918"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li><li class="menu-item  menu-item-label pull-right no-margin-left dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Java</li><li class="menu-item  menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Line 1, Column 1</li><li class="menu-item  menu-item-label dropdown-header"><i class="menu-icon fa fa-sign-blank"></i>Normal Keyboard</li><li class="menu-item  menu-item-menu no-margin dropdown-submenu"><a href="#" testid="command14030" tabindex="-1"><i class="menu-icon fa fa-sign-blank"></i>Syntax</a></li><li class="menu-item  menu-item-action"><a href="#" testid="command14518"><i class="menu-icon fa fa-sign-blank"></i>https://10-142-0-44-8000-9d1qqkklgmp-2e7g.hackerrank.io</a></li></ul></div>
</div>
<div class="cb-loading-alert" style="display: none;"><div class="cb-loadings-spinner"></div><div class="cb-loading-message"></div><div class="cb-loading-sub-message"></div></div>

<!-- <div class="cb-loading-alert"><div class="cb-loadings-spinner"></div><div class="cb-loading-message"></div></div> -->

<!-- <div id="codekit">
	<div class="cb-login">
		<div class="login-box">
			<div class="header">
  				<img src="static/images/icons/128.png" />
			</div>
			<form class="inner">
				

				
					<div class="form-group">
						<input type="email" class="form-control input-lg" name="login-email" id="login-email" placeholder="Email" value="6673040" autocomplete="off">
						
						<p class="help-block">This workspace is public, enter an email to identify yourself (GIT and collaborators).</p>
						
					</div>
					
					<button id="login-submit" class="btn btn-lg btn-block btn-default">Enter</button>
				
			</form>
		</div>
	</div>
</div> -->
</div>
</div>

    </div></div>
      <div class="clear"></div>
      
        <button class="btn btn-primary mdT mdB mdR ans-submit pull-right" style="width:250px;">Submit code &amp; continue</button>
        <button class="btn btn-default mdT mdB mdR run-tests pull-right">Run Tests</button>
        <div class="clear gray pull-right mdR" style="padding-top: 10px;  text-align: left;">You can change your submission later.</div>
      
    
  </div>