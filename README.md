The source code that generated this unhandled exception can only be shown when compiled in debug mode. To enable this, please follow one of the below steps, then request the URL:

1. Add a "Debug=true" directive at the top of the file that generated the error. Example:

<%@ Page Language="C#" Debug="true" %>

2) Add the following section to the configuration file of your application:

<configuration>

<system.web> <compilation debug="true"/> </system.web>

</configuration>

Note that this second technique will cause all files within a given application to be compiled in debug mode. The first technique will cause only that particular file to be compiled in debug mode.

Important: Running applications in debug mode does incur a memory/performance overhead. You should make sure that an application has debugging disabled before deploying into production scenario.

Client IP:

Port: 48942

Referer:

Path:

User-Agent: Mozilla/5.0

ViewState:

110.227.61.186

https://ssvmexam.in/UG_NEP_RE

SULT.aspx

/UG_NEP_RESULT.aspx

(Linux; Android 10; K)

AppleWebKit/537.36 (KHTML, like Gecko) Chrome/154.0.0.0 Mobile Safari/537.36

U/6K/oPxEC6D3rfWAvKNVk820rzUFd+ y/wx1AT3PFdyRJYQPqbaBsLfxAp+Yr6 ReMWiMISf1BMZF2ur/1T7kZDw0olpP+ 8h1Hbrx25zqkooEeehTLs9Q3nGtLqcy JzQXPcggqD1PJkx/mC79D4ZNNe9A8wL wltNpIr4NF44XSf8hnWaBtu8mKEH3Ka hw2GkYWBGw4Mm1a6m2PAzN7lIwuScTK 1cU7ci9bVYEQjEAcS7Yo3ItEdYy6NZM o39taONw2ssUFwf2fLouzoA2S8bHa+C 8f/XBkSBKVTJ07aN3qPc08RrzrvLJ/v QsBrKIFUqnFU9qqoptRGK8yHCRiioST YDA87YIVT30SVS/1QBdG2JUXUtARcDh kmMfu5qSHNGDl+kmCz7A0Cu39IX92LB DLOpiS1mbOfF2P7r+/R/+FZ6ZCXNnAB 7Jt3vfKteYGLPQ0fhxQ48SREDMq2lCF HIG4D19ubr+akQAhjAwQabNDQgR3r1R 2ifHhCefP5CTOZZJCSLl0gqYcTPKAju oSwtmlXfE1SCc2/dHLZv3cIH/w8MsSC zjiTKM5vjz+Ci/9TrKyFnFlL+3cx4Pm
2deHnFaWsCCf4qu...]

[HttpException (0x80004005): Validation of viewstate MAC failed. If this application is hosted by a Web Farm or cluster, ensure that <machineKey> configuration specifies the same validationKey and validation algorithm. AutoGenerate cannot be used in a cluster.

See http://go.microsoft.com/fwlink/?LinkID=314055 for more information.]

System.Web.UI.ViewStateExceptio n. ThrowError (Exception inner, String persistedState, String errorPageMessage, Boolean macValidationError) +161

System.Web.UI.ObjectStateFormat ter. Deserialize(String inputString, Purpose purpose) +731

System.Web.UI. Util.DeserializeW ithAssert(IStateFormatter2 formatter, String serializedState, Purpose purpose) +65

System.Web.UI.HiddenFieldPageSt atePersister. Load() +319

System.Web.UI.Page. LoadPageStat eFromPersistenceMedium() +377
System.Web.UI.Page.ProcessReque stMain(Boolean includeStagesBeforeAsyncPoint, Boolean includeStages AfterAsyncPoint) +9298

System.Web.UI.Page.ProcessReque st(Boolean includeStages BeforeAsyncPoint, Boolean includeStages AfterAsyncPoint) +355

System.Web.UI.Page.ProcessReque st() +79

System.Web.UI.Page.ProcessReque st(HttpContext context) +74

ASP.ug_nep_result_aspx.ProcessR equest(HttpContext context) +46

System.Web.CallHandlerExecution Step.System.Web.HttpApplication .IExecutionStep.Execute() +537

System.Web.HttpApplication.Exec uteStepImpl(IExecutionStep step) +172

System.Web.HttpApplication.Exec uteStep (IExecutionStep step, Boolean& completedSynchronously) +93
<a href="class5.pdf">कक्षा 5वीं का परिणाम देखें</a>
<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>विद्यालय परीक्षा परिणाम</title>
<style>
body {
  font-family: Arial, sans-serif;
  background: #eef3ff;
  margin: 0;
  padding: 15px;
}
header {
  background: #123c69;
  color: white;
  text-align: center;
  padding: 20px 10px;
  border-radius: 12px;
}
.box {
  background: white;
  max-width: 500px;
  margin: 20px auto;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 2px 10px #cccccc;
}
label, select, input, button {
  display: block;
  width: 100%;
  box-sizing: border-box;
  margin-top: 12px;
  padding: 12px;
  font-size: 16px;
}
button {
  background: #123c69;
  color: white;
  border: none;
  border-radius: 6px;
}
#result {
  margin-top: 20px;
  overflow-x: auto;
}
table {
  width: 100%;
  border-collapse: collapse;
}
td, th {
  border: 1px solid #ccc;
  padding: 8px;
  text-align: center;
}
footer {
  text-align: center;
  margin-top: 25px;
  color: #555;
}
</style>
</head>
<body>

<header>
  <h2>शिशु</h2>
  <h3>विद्यालय</h3>
  <p>परीक्षा परिणाम 2026</p>
</header>

<div class="box">
  <h3>अपना परिणाम देखें</h3>

  <label for="class">अपनी कक्षा चुनें</label>
  <select id="class">
    <option value="">कक्षा चुनें</option>
    <option>5</option>
    <option>6</option>
    <option>7</option>
    <option>8</option>
  </select>

  <label for="roll">रोल नंबर डालें</label>
  <input id="roll" type="number" placeholder="अपना रोल नंबर">

  <button onclick="showResult()">परिणाम देखें</button>
  <div id="result"></div>
</div>

<footer>
  <p>विद्यालय</p>
</footer>

<script>
function showResult() {
  const cls = document.getElementById("class").value;
  const roll = document.getElementById("roll").value;
  const result = document.getElementById("result");

  if (!cls || !roll) {
    result.textContent = "कृपया कक्षा और रोल नंबर दोनों भरें।";
    return;
  }

  result.textContent =
    "रोल नंबर " + roll +
 ";
}
</script>
</body>
</html>
https://ssvmexam.in/UG_NEP_RE