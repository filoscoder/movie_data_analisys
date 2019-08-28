# Movie Dataset Downloader
<h6>Personal project written on VS Code and run on linux (CentOS7)</h6>

<h2><dataset-downloader></h2>
  <p><b>dataset-downloader</b> as his name, it is a simple dataset downloader based on unix eviroment
  It automates the downloads of movies related data from the <i>Korean Film Counsil</i> (kobis.or.kr)
  This program downloads 2 type of dataset:
  <ol><li> Daily box office dataset </li>
    <li> Detailed movie info dataset (Movies those are included at the daily box office dataset) </li>
  </ol></p>
 
 <h3><Dev enviroment></h3>
  Bash file written on <b>VS Code</b>
  <b>Linux</b> terminal(CentOS7)
  <b>.JQ</b> line editor for Json files

<h4>Instruccions</h4>
<ul>
  *REQUISITE: <b>MUST</b> have all permission granted to <i>read/write/run</i> (rwx)
  <li> Open your terminal on Linux </li>
  <li> Go to your preferred workspace and create a new directory called '<b>movies_data</b>'</li>
  <code>MKDIR -pv /{$WORKSPACE PATH}/movies_data</code>
  <li> Web download ('wget' command) the current latest version: <a href='https://raw.githubusercontent.com/filoscoder/movie_data_analisys/master/dataset-downloader-1.2.sh'>dataset-downloader-1.2.sh</a></li>
  <code>wget -p /{$WORKSPACE PATH}/ https://raw.githubusercontent.com/filoscoder/movie_data_analisys/master/dataset-downloader-1.2.sh </code>
  <li>Grant full access to the downloader file</li>
  <code>chmod 777 dataset-downloader-1.2.sh </code>
  <li>Run the file and Enjoy!</li>
  <code> ./dataset-downloader-1.2.sh </code>
  <li><em>If you experience some syntax issues try again after this</em></li>
  <code> sed -i 's/\r$//g' /home/hadoop/movies_data/dataset-downloader-1.2.sh</code>
  <i>this issue happend because the bash file was written on windows and linux interprete the 'Enter' key like '\r' (carriage return)
    so the code above use the stream line editor to remove every '\r' on the file.</i>
  <em>If you keep have troubles running the downloader, please send me an email (sondaniel.88@gmail.com) </em>

  
  <h4>Change Log</h4>
<ul>
  <strong><b># v1.2 <b/></strong>
  <li> Added .jq editor installer (if not yet installed) </li>
  <li> Fixed minor issues </li>
  <strong><b># v1.1 <b/></strong>
    <li> Changed the download path and the downloaded filenames to 'YYYYMMDD' </li>
    <li> Handled wrong user input format </li>
    <li> Fixed unnecessary downloads about existing files </li>
  <strong># v1.0 <b/></strong>
    <li> Initial release </li>
</ul>
