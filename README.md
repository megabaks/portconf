portconf
========

/etc/portage cleaner

USE:
	<ul>
	<li>package.use</li>
		<ul>
			<li>Find and remove incorrect.Checking flags for ALL available versions ( hello, portpeek :3 ).</li>
			<li>Find and remove flags, which present in make.conf/profile and have the same state.</li>
			<li>Sort: remove doubles and preserve only last defined state (on/off).</li>
			<li>Merge: all flags in one line per atom ("<>=~" switches depend).</li>
		</ul>
	<li>make.conf</li>
		<ul>
			<li>Find and remove flags, which defined in profile and have the same state.</li>
		</ul>
	</ul>
ATOMS:
	<ul>
		<li>Find and remove incorrect/not_founded/not_installed.( in /etc/portage/env too ).</li>
	</ul>
Features:
	<ul>
		<li>Auto backup (make.conf included).</li>
		<li>Rebuild: package.* from flat files to dirs and back.</li>
		<li>Sort atoms alphabetically</li>
		<li>/etc/portage/make.conf override /etc/make.conf ( as portage ).</li>
	</ul>
