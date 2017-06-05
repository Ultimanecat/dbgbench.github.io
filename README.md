## Summary
How do professional software engineers debug computer programs? In an experiment with 27 real bugs that existed in several widely used programs, we invited 12 professional software engineers, who together spent one month on localizing, explaining, and fixing these bugs. This did not only allow us to study the various tools and strategies used to debug the same set of errors. We could also determine exactly which statements a developer would localize as faults, how a developer would diagnose and explain an error, and how a developer would fix an error – all of which software engineering researchers seek to automate. Until now, it has been difficult to evaluate the effectiveness and utility of automated debugging techniques without a user study. We publish the collected data, called DBGBENCH, to facilitate the effective evaluation of automated fault localization, diagnosis, and repair techniques w.r.t. the judgement of human experts.

<p style="position:fixed; left: 50%; top: 255px; transform: translate(-635px, 0%); width: 300px; padding: 0px">
<a href="#use">Use DBGBench</a><br/>
<a href="#cite">Cite DBGBench</a><br/>
<a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/abstract.pdf"><img src="https://github.com/dbgbench/dbgbench.github.io/raw/master/abstract.png" alt="DBGBench Abstract" style="width: 300px;"/></a></p>

<p align="center"><img src="https://github.com/dbgbench/dbgbench.github.io/raw/master/mainobjective.png" alt="Main Objectives" width="90%" /></p>

| Descriptive Statistics | Benchmark Details |
| -- | -- |
| **<a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/benchmark.pdf" target="_blank">[find.24e2271e]</a>**<br/>*Error Type*: Functional Bug<br/>*Avg. Time*: 13.8 min<br/>*Explanation*: Slightly difficult<br/>*Patching*: Slightly difficult<br/>*Correctness*: 75% | *Regression*: <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=f0759ab8db9cab16699fba45fa6117ef06620194" target="_blank">Commit</a><br/>*Bug Report*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.24e2271e.report.txt" target="_blank">Simple</a>, [Original](http://savannah.gnu.org/bugs/?18222)<br/>*Fault Locations*: Here<br/>*Bug Diagnosis*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.24e2271e.diagnosis.txt" target="_blank">Here</a><br/>*Patches*: Participants <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=24e2271ec05c9b5a5517a76d3756af417a637e95" target="_blank">Developers</a><br/>*Tests*: Here |
| **<a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/benchmark.pdf" target="_blank">[find.dbcb10e9]</a>**<br/>*Error Type*: Crash<br/>*Avg. Time*: 22.9 min<br/>*Explanation*: Slightly difficult<br/>*Patching*: Slightly difficult<br/>*Correctness*: 81%| *Regression*: <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=daf7f100ed3cc056b6cfad04435f8ae879587f67" target="_blank">Commit</a><br/>*Bug Report*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.dbcb10e9.report.txt" target="_blank">Simple</a>, [Original](http://savannah.gnu.org/bugs/?20139)<br/>*Fault Locations*: Here<br/>*Bug Diagnosis*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.dbcb10e9.diagnosis.txt" target="_blank">Here</a><br/>*Patches*: Participants <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=dbcb10e9f939a649a7ba99a1fec39eb01e40fde2" target="_blank">Developers</a><br/>*Tests*: Here |
| **<a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/benchmark.pdf" target="_blank">[find.07b941b1]</a>**<br/>*Error Type*: Crash<br/>*Avg. Time*: 23.7 min<br/>*Explanation*: Slightly difficult<br/>*Patching*: Slightly difficult<br/>*Correctness*: 80% | *Regression*: <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=84aef0ea1170af8910613c39e98e05505c7c03d0" target="_blank">Commit</a><br/>*Bug Report*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.07b941b1.report.txt" target="_blank">Simple</a>, [Original](http://savannah.gnu.org/bugs/?17490)<br/>*Fault Locations*: Here<br/>*Bug Diagnosis*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.07b941b1.diagnosis.txt" target="_blank">Here</a><br/>*Patches*: Participants <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=07b941b1e71a2212b8fd2d3a32662aa5dbfdfa8b" target="_blank">Developers</a><br/>*Tests*: Here |
| **<a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/benchmark.pdf" target="_blank">[find.c8491c11]</a>**<br/>*Error Type*: Crash<br/>*Avg. Time*: 31.4 min<br/>*Explanation*: Slightly difficult<br/>*Patching*: Slightly difficult<br/>*Correctness*: 54%| *Regression*: <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=864b25ed9c1f9f87c036196cb70a7cc21357207b" target="_blank">Commit</a><br/>*Bug Report*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.c8491c11.report.txt" target="_blank">Simple</a>, [Original](http://savannah.gnu.org/bugs/?24169)<br/>*Fault Locations*: Here<br/>*Bug Diagnosis*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find.c8491c11.diagnosis.txt" target="_blank">Here</a><br/>*Patches*: Participants <a href="http://git.savannah.gnu.org/cgit/findutils.git/commit/?id=c8491c11d581598348f034dc55e51e12ee46159a" target="_blank">Developers</a><br/>*Tests*: Here |


```
| **<a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/benchmark.pdf" target="_blank">[find.]</a>**<br/> | *Regression*: <a href="" target="_blank">Commit</a><br/>*Bug Report*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find. .report.txt" target="_blank">Simple</a>, [Original]( )<br/>*Fault Locations*: Here<br/>*Bug Diagnosis*: <a href="https://github.com/dbgbench/dbgbench.github.io/raw/master/find. .diagnosis.txt" target="_blank">Here</a><br/>*Patches*: Participants <a href="" target="_blank">Developers</a><br/>*Tests*: Here |
```

## <a name="use"></a>How to Use?

## <a name="cite"></a>How to Cite?
```
@inproceedings{dbgbench, 
  author = {B\"{o}hme, Marcel and Soremekun, Ezekiel Olamide and Chattophadyay, Sudipta and Ugherughe, Emamurho and Zeller, Andreas}, 
  title = {Where is the Bug and How is it Fixed? An Experiment with Practitioners}, 
  booktitle = {Proceedings of the Joint meeting of the European Software Engineering Conference and the ACM SIGSOFT Symposium on the Foundations of Software Engineering (ESEC/FSE) 2017}, 
  series = {FSE 2017}, 
  pages = {1-11}, 
  year = {2017}
}
```


