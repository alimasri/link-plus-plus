# Link++
<h3>Introduction</h3>
Existing interlinking tools focus on finding similarity relationships between entities of distinct RDF datasets by generating owl:sameAs links.
These approaches address the detection of equivalence relations between entities.
However, in some contexts, more complex relations are required, and the links to be defined follow more sophisticated patterns.
We introduce <b>Link++</b>, an approach that enables the discovery of complex links in a flexible manner.
<b>Link++</b> enables the users to generate rich links by defining custom functions and linking patterns that fit their needs.
<hr />
<h3>Instructions</h3>
This repository contains the executable file link_pp.jar that can be launched via the command: java -cp link_pp.jar app.cli.Application
After running the command the program will show its usages.
In addition to the executable file we have included the following files as a sample scenario:
<ul>
  <li><i>sncf.ttl</i> a turtle file containing data about SNCF's stop locations. SNCF is a railway company in France see http://www.sncf.com/.
  The data was downloaded from http://gtfs.s3.amazonaws.com/sncf_20131211_1451.zip
  </li>
  <li><i>velib.ttl</i> a turtle file containing data about VELIB's bike station data. VELIB is a bike sharing company in France http://en.velib.paris.fr/. The data was downloaded from http://opendata.paris.fr/explore/dataset/stations-velib-disponibilites-en-temps-reel/
  </li>
  <li><i>linking-rule</i> a sample linking rule with a goal of connecting data entities that are X kilometers apart.
  Note that this file can be changed to fit any other linking task based on the user's need</li>
  <li><i>output-pattern</i> a sample file specifying what connection pattern a user wants as an output for a given matching task.
  In this scenario the output pattern generated information about the calculated distance and the duration between two transportation entities.
  <li><i>classes</i> a folder containing a compiled version of any function a user needs for a linking task.
  Users may use any external library as well but it is required that the used library exists in the classes folder.</li>
  <li><i>output</i> a folder containing the output of a linking process</li>
</ul>