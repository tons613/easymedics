<HTML>
  <HEAD>
    <TITLE>EasyMedics</TITLE>
    <META HTTP-EQUIV="Content-Type" CONTENT="text/html; charset=utf-8" />
   

<SCRIPT LANGUAGE="JavaScript">
runtimeVersion = "4.0.0";
checkClient = false;
directLink = "EasyMedics.application";


function Initialize()
{
  if (HasRuntimeVersion(runtimeVersion, false) || (checkClient && HasRuntimeVersion(runtimeVersion, checkClient)))
  {
    InstallButton.href = directLink;
    BootstrapperSection.style.display = "none";
  }
}
function HasRuntimeVersion(v, c)
{
  var va = GetVersion(v);
  var i;
  var a = navigator.userAgent.match(/\.NET CLR [0-9.]+/g);
  if(va[0]==4)
    a = navigator.userAgent.match(/\.NET[0-9.]+E/g);
  if (c)
  {
    a = navigator.userAgent.match(/\.NET Client [0-9.]+/g);
    if (va[0]==4)
       a = navigator.userAgent.match(/\.NET[0-9.]+C/g);
  }
  if (a != null)
    for (i = 0; i < a.length; ++i)
      if (CompareVersions(va, GetVersion(a[i])) <= 0)
                                return true;
  return false;
}
function GetVersion(v)
{
  var a = v.match(/([0-9]+)\.([0-9]+)\.([0-9]+)/i);
  if(a==null)
     a = v.match(/([0-9]+)\.([0-9]+)/i);
  return a.slice(1);
}
function CompareVersions(v1, v2)
{
   if(v1.length>v2.length)
   {
      v2[v2.length]=0;
   }  
   else if(v1.length<v2.length)
   {
      v1[v1.length]=0;
   }

  for (i = 0; i < v1.length; ++i)
  {
    var n1 = new Number(v1[i]);
    var n2 = new Number(v2[i]);
    if (n1 < n2)
      return -1;
    if (n1 > n2)
      return 1;
  }
  return 0;
}

</SCRIPT>

</HEAD>
  <BODY ONLOAD="Initialize()">
    <TABLE WIDTH="100%" CELLPADDING="0" CELLSPACING="2" BORDER="0">


<!-- Begin Dialog -->
<TR><TD ALIGN="LEFT"><TABLE CELLPADDING="2" CELLSPACING="0" BORDER="0" WIDTH="540"><TR><TD WIDTH="496">

<!-- Begin AppInfo -->
<TABLE><TR><TD COLSPAN="3">&nbsp;</TD></TR><TR><TD><B>Name:</B></TD><TD WIDTH="5"><SPACER TYPE="block" WIDTH="10" /></TD><TD>EasyMedics</TD></TR><TR><TD COLSPAN="3">&nbsp;</TD></TR><TR><TD><B>Version:</B></TD><TD WIDTH="5"><SPACER TYPE="block" WIDTH="10" /></TD><TD>4.3.1.10</TD></TR><TR><TD COLSPAN="3">&nbsp;</TD></TR><TR><TD><B>Publisher:</B></TD><TD WIDTH="5"><SPACER TYPE="block" WIDTH="10" /></TD><TD>A-One GlobalSoft Technologies</TD></TR><tr><td colspan="3">&nbsp;</td></tr></TABLE>
<!-- End AppInfo -->


<!-- Begin Prerequisites -->
<TABLE ID="BootstrapperSection" BORDER="0"><TR><TD COLSPAN="2">The following prerequisites are required:</TD></TR><TR><TD WIDTH="10">&nbsp;</TD><TD><UL>
<LI>Microsoft .NET Framework 4 (x86 and x64)</LI>
<LI>Windows Installer 3.1</LI>
</UL></TD></TR><TR><TD COLSPAN="2">
If these components are already installed, you can <SPAN CLASS="JustThisApp"><A HREF="EasyMedics.application">launch</A></SPAN> the application now. Otherwise, click the button below to install the prerequisites and run the application.
</TD></TR><TR><TD COLSPAN="2">&nbsp;</TD></TR></TABLE>
<!-- End Prerequisites -->


</TD></TR></TABLE>
<!-- Begin Buttons -->
<TR><TD ALIGN="LEFT"><TABLE CELLPADDING="2" CELLSPACING="0" BORDER="0" WIDTH="540" STYLE="cursor:hand" ONCLICK="window.navigate(InstallButton.href)"><TR><TD ALIGN="LEFT"><TABLE CELLPADDING="1" BGCOLOR="#333333" CELLSPACING="0" BORDER="0"><TR><TD><TABLE CELLPADDING="1" BGCOLOR="#cecece" CELLSPACING="0" BORDER="0"><TR><TD><TABLE CELLPADDING="1" BGCOLOR="#efefef" CELLSPACING="0" BORDER="0"><TR><TD WIDTH="20"><SPACER TYPE="block" WIDTH="20" HEIGHT="1" /></TD><TD><A ID="InstallButton" HREF="setup.exe">Install</A></TD><TD width="20"><SPACER TYPE="block" WIDTH="20" HEIGHT="1" /></TD></TR></TABLE></TD></TR></TABLE></TD></TR></TABLE></TD><TD WIDTH="15%" ALIGN="right" /></TR></TABLE></TD></TR>
<!-- End Buttons -->
</TD></TR>
<!-- End Dialog -->



<!-- Spacer Row -->
<TR><TD>&nbsp;</TD></TR>

<TR><TD>
<!-- Begin Footer -->
<TABLE WIDTH="100%" CELLPADDING="0" CELLSPACING="0" BORDER="0" BGCOLOR="#ffffff"><TR><TD HEIGHT="5"><SPACER TYPE="block" HEIGHT="5" /></TD></TR><TR><TD CLASS="FooterText" ALIGN="center">
<A HREF="http://globalsoft.com.ng">A-One GlobalSoft Technologies Customer Support</A>
&nbsp;&nbsp;&nbsp;::&nbsp;&nbsp;&nbsp;
<A HREF="https://go.microsoft.com/fwlink/?LinkId=154571">ClickOnce and .NET Framework Resources</A>
</TD></TR><TR><TD HEIGHT="5"><SPACER TYPE="block" HEIGHT="5" /></TD></TR><TR><TD HEIGHT="1" bgcolor="#cecece"><SPACER TYPE="block" HEIGHT="1" /></TD></TR></TABLE>
<!-- End Footer -->
</TD></TR>

</TABLE>
  </BODY>
</HTML>