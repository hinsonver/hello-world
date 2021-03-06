# CrowdDEC 
<ul>
    <li> <a href ="#a1">Documentation</a>
    <li> <a href ="#a2">Building</a>
    <li> <a href ="#a3">Main Code Directory Structure</a>
    <li> <a href ="#a4">Test Code Directory Structure</a>
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
##<a id="a3" name="a3"></a>Main Code Directory Structure  
<strong>core</strong>   
The main content of the CrowdDEC algorithm.  
<strong>&nbsp;&nbsp;estimate</strong><br>
<a>&nbsp;&nbsp;5 kinds of worker model estimation methods (AbsoluteDiscount, Empirical, GoodTuring, Hybrid, JelinekMercer)<a>  
<strong>&nbsp;&nbsp;select</strong><br>
<a>&nbsp;&nbsp;5 kinds of worker selection algorithms (BestEffort, BruteForce, GreedyInsert, LocalSearch, Random)<a><br>
<strong>&nbsp;&nbsp;CrowdDEC.java</strong><br>
<a>&nbsp;&nbsp;CrowdDEC framework.<a><br>
<strong>&nbsp;&nbsp;CrowdQEC.java</strong><br>
<a>&nbsp;&nbsp;Quotas crowdsourced entities collection framework,for comparing with CrowdDEC.<a><br>
<strong>&nbsp;&nbsp;Distribution.java</strong><br>
<a>&nbsp;&nbsp;Definition of entity distribution.<a><br>
<strong>&nbsp;&nbsp;WorkerModel.java</strong><br>
<a>&nbsp;&nbsp;Crowd model for CrowdDEC.<a><br>
<strong>worker</strong>  
Operations of the Crowdsourced workers.<br>
<strong>&nbsp;&nbsp;AMTWorker.java</strong><br>
<a>&nbsp;&nbsp;Matches the workers and their submit timepoints.<a><br>
<strong>&nbsp;&nbsp;AMTWorkerPool.java</strong><br>
<a>&nbsp;&nbsp;Obtain all vaild workers and the entities they submit.<a><br>
<strong>&nbsp;&nbsp;WorkerPool.java</strong><br>
<a>&nbsp;&nbsp;Defines 3 abstract methods of worker operations.<a><br>
<strong>util</strong>  
Tool set.  
<strong>&nbsp;&nbsp;Domain.java</strong><br>
<a>&nbsp;&nbsp;Codes for workers and entities.<a><br>
<strong>&nbsp;&nbsp;Histogram.java</strong><br>
<a>&nbsp;&nbsp;Plots histograme.<a><br>
<strong>&nbsp;&nbsp;KL.java</strong><br>
<a>&nbsp;&nbsp;Compute the KL distance between the entity distribution.<a><br>
<strong>&nbsp;&nbsp;ScoredItem.java</strong><br>
<a>&nbsp;&nbsp;Sort tool.<a><br>
<strong>launchers</strong>  
Run the programe.  
##<a id="a4" name="a4"></a>Test Code Directory Structure 
<strong>PseudoWorker.java</strong><br>
<a>&nbsp;&nbsp;Creates a pseudo worker set.<a><br>
<strong>RunningExample.java</strong><br>
<a>&nbsp;&nbsp;A test running file.<a><br>
<strong>SimuEnv.java/SimuAssignEval.java</strong><br>
<a>&nbsp;&nbsp;The test file of worker selection methods.<a><br>
##<a id="a5" name="a5"></a>Data
 We conduct experiments on the well-known crowdsourcing platform Amazon Mechanical Turk (AMT) and evaluate the approaches on two real datasets collected from the workers on AMT.  
 
(1) The movie dataset contains a set of movie entities: each worker is asked to submit movies she knows, together with an attribute decade indicating the time a movie firstly publishes. The domain of this attribute contains 7 distinct values, ranging from 1950s to 2010s.  
(2) The car dataset contains a set of car entities from the workers, together with an attribute body style which has15 distinct values, such as sedans , suvs , etc.

