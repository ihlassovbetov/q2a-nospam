# q2a-nospam
<b>Plugin Name:</b>  NoSpam <br>
<b>Price:</b> 30 USD (contact me to buy) <br>
<b>Plugin Description:</b> This is a premium-paid Q2A plugin that various methods to prevent spam registrations. It will filter 100% non-human registration.<br>
<br>
<ul class="first">
	<b>Plugin Functionality:</b>
	<li>Plugin creates a table in database to store data.</li>
	<li>Plugin offers various methods to combat with spammers:
		<ul class="second">
			<li><b>ONLY ALLOWED EMAIL PROVIDERS (WHITELISTED):</b> admin can set which email providers are allowed. Spammers tend to use non-common email providers. So, it will partly filter them out.</li>
			<li><b>CHECK UPPERCASE CHARACTERS:</b> admin can enable this to check if users input email comprises uppercase characters (spam emails tend to have uppercase lettes).</li>
			<li><b>ADD NO-FILL INPUT:</b> it is hidden no fill input inserted on registration page. Spam bots tend to fill all input elements in the form, so it will mislead them.</li>
			<li><b>ADD CUSTOM ANTI-SPAM QUESTION:</b> admin can add a set of anti-spam questions with its answers. On each register page load, the script will randomly select one of anti-spam questions and ask users to answer it. This will prevent majority of spam registration if number of questions are high.</li>
			<li><b>CONFIRMATION LINK BEFORE REGISTRATION:</b> when user attempt to register, it will generate 8 digits alfanumeric code and store all input data (handle, password, email, code) in to a temporary database table with current time (starttime) and time 24 hours later (endtime). And script will send email with confirmation link to the users email address. The user needs to click that email within 24 hours (before endttime, which is expire time). Once user clicks that link within 24 hours then REAL Q2A REGISTRATION (add row to users database table) will be processed and temporary row at database table will be immediately deleted. If user fails to click that link then after link will expire after 24 hours and the users row on temporary database table will be automatically removed. (It will need manual set of cronjob (daily check) at server side.)</li>
		</ul>
	</li>
	<li>Admin can enable/disable each above methods.</li>
	<br/>
	<img src="https://ihlassovbetov.github.io/assets/plugin-ss/nospam/img-1.png" width="500px" height="auto" />
	<img src="https://ihlassovbetov.github.io/assets/plugin-ss/nospam/img-2.png" width="500px" height="auto" />
</ul>
<br/>
<ul class="first">	
	<b>TEST DEMO WEBSITE: <a href="https://www.e-dostluk.com/q2a-demo" target="_blank">LIVE DEMO</a></b>
	<li>Standard registered user (username: deneme_11 / pass: test1234)</li>
	<li>Moderator user (username: demo / pass: demo1234)</li>
</ul>

