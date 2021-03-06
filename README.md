jQuery UI Dialog Titlebar Help button Plugin
======================

is a plug-in to add a Help button in the title bar of the dialog.
If you want to use with visual studio you can take advantage of NuGet.

Sample Code
----------

``` html
<html>
<head>
	<script type="text/javascript" src="http://code.jquery.com/jquery-1.7.2.min.js"></script>
	<script type="text/javascript" src="http://code.jquery.com/ui/1.8.19/jquery-ui.min.js"></script>
	<script type="text/javascript" src="../jquery.dialog.helpbutton.js"></script>
	<script type="text/javascript">
		$(function(){
			$('#dialog1').dialog({
				/* jquery UI Dialog options */
				autoOpen: false,
				modal: true,
				resizable: false,
				width: 200,
				height: 200,
				/* dialog.helpbutton options */
				help: 'testHelp.html'
			});
			$('#dialogOpen1').click(function() {
				$('#dialog1').dialog('open');
			});
		});
	</script>
	<link href="http://code.jquery.com/ui/1.8.19/themes/base/jquery-ui.css" rel="stylesheet"/>
	<link href="../jquery.dialog.helpbutton.css" rel="stylesheet"/>
</head>
<body>
	<a id="dialogOpen1" href="#">Dialog Open</a>
	<div id="dialog1" title="Sample">
		dialog<br/>
		<br/>
		contents
	</div>
</body>
</html>
```

Option
----------
+   `help` :
    Sets the url of the Help page.
    Unset does not display the button.
    
+   `helpTitle` :
    help page window title.

License
----------
Copyright &copy; 2012 MiYABiS
Distributed under the [MIT License][mit].
 
[MIT]: http://www.opensource.org/licenses/mit-license.php
