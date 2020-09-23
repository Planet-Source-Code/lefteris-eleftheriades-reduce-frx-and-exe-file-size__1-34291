<div align="center">

## Reduce Frx and Exe file size


</div>

### Description

Did you that your Frx files and Exe files, may be bigger in size than they were supposed to?

(Note: I have submitted this artical befoure but it got deleted. I don't know how.)

Please Vote
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Lefteris Eleftheriades](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/lefteris-eleftheriades.md)
**Level**          |Advanced
**User Rating**    |4.4 (44 globes from 10 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Data Structures](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/data-structures__1-33.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/lefteris-eleftheriades-reduce-frx-and-exe-file-size__1-34291/archive/master.zip)





### Source Code

<p style="margin-top: 0; margin-bottom: 0"><font size="5" color="#FF0000">S.O.S
about Frx and Exe file size</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font size="4" color="#0000FF">In
some cases, the size of FRX and EXE files is higher than it should be.</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font size="4">These cases only
involve forms with <b>picture-box </b>&nbsp;controls which contain pictures and</font></p>
<p style="margin-top: 0; margin-bottom: 0"><font size="4">These pictures have
been <b>changed</b> at least once (Replaced by a new picture)</font></p>
<p style="margin-top: 0; margin-bottom: 0">&nbsp;</p>
<p style="margin-top: 0; margin-bottom: 0">This is caused because Visual Basic
saves all binary data (Such as pictures) in the</p>
<p style="margin-top: 0; margin-bottom: 0">end of the form's FRX file. Now, If
you change a picture-box's picture property to a new picture the old picture
will <u>not be overwritten</u>, and <u>still allocate space</u> in the frx file.</p>
<p style="margin-top: 0; margin-bottom: 0">This problem also <u>effects the
compiled EXE</u> file which saves all the data from the frx file.</p>
<p style="margin-top: 0; margin-bottom: 0">&nbsp;</p>
<p style="margin-top: 0; margin-bottom: 0">In a game is was doing I had to
change the Picture of an image control that contained the</p>
<p style="margin-top: 0; margin-bottom: 0">Background image many times.</p>
<p style="margin-top: 0; margin-bottom: 0">&nbsp;</p>
<p style="margin-top: 0; margin-bottom: 0"><font size="4">Findings:</font></p>
<p style="margin-top: 0; margin-bottom: 0"><b>Frx File size: 1.14 MB</b></p>
<p style="margin-top: 0; margin-bottom: 0"><b>Exe File size: 1.83 MB</b></p>
<p style="margin-top: 0; margin-bottom: 0">&nbsp;</p>
<p style="margin-top: 0; margin-bottom: 0">Then I deleted the Form1.frx file and
set the pictures again.</p>
<p style="margin-top: 0; margin-bottom: 0">&nbsp;</p>
<p style="margin-top: 0; margin-bottom: 0"><font size="4">Findings:</font></p>
<p style="margin-top: 0; margin-bottom: 0"><b>Frx File size: 0.340 MB (340KB
only!!!)</b></p>
<p style="margin-top: 0; margin-bottom: 0"><b>Exe File size: 0.412 MB (412 KB
only!!!)</b></p>
<p style="margin-top: 0; margin-bottom: 0">&nbsp;</p>
<p style="margin-top: 0; margin-bottom: 0"><font size="4">Conclusion:</font></p>
<p style="margin-top: 0; margin-bottom: 0">After making a lot of changes in a
program you make, and the changes concern binary data (Pictures, Ole container
data) always delete the FRX files and set the properties from squad.</p>

