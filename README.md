# CrowdDEC
<ul>
    <li> <a href ="#a1">Documentation</a>
    <li> <a href ="#a2">Building</a>
    <li> <a href ="#a3">Main code file structure</a>
    <li> <a href ="#a4">Test code file structure</a>
    <li> <a href ="#a5">Data</a>
## <a id="a1" name="a1"></a>[Documentation] ()
## <a id="a2" name="a2"></a>Building  
Use Apache Maven 3.0 to build this project
###Step 1  
    mvn clean install
###Step 2  
    mvn compile
###Step 3  
    mvn test 
##<a id="a3" name="a3"></a>Main code file structure  
<strong>core<br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;estimate<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;select </strong><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CrowdDEC.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;CrowdQEC.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Distribution.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;WorkerModel.java<a><br>
<strong>worker</strong><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AMTWorker.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AMTWorkerPool.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;WorkerPool.java<a><br>
<strong>util</strong><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Domain.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Histogram.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;KL.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ScoredItem.java<a><br>
<strong>&nbsp;launchers</strong><br>
##<a id="a4" name="a4"></a>Test code file structure 
<a>PseudoWorker.java<a><br>
<a>RunningExample.java<a><br>
##<a id="a5" name="a5"></a>Data
 <p>We conduct experiments on the well-known crowdsourcing platform Amazon Mechanical Turk (AMT) and evaluate the approaches on two real datasets collected from the workers on AMT.</p>  
(1) The movie dataset contains a set of movie entities: each worker is asked to submit movies she knows, together with an attribute decade indicating the time a movie firstly publishes. The domain of this attribute contains 7 distinct values, ranging from 1950s to 2010s.  
(2) The car dataset contains a set of car entities from the workers, together with an attribute body style which has15 distinct values, such as sedans , suvs , etc.

