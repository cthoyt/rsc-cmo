# CHMO

The Chemical Methods Ontology contains more than 3000 classes and describes methods used to:
* collect data in chemical experiments, such as mass spectrometry and electron microscopy 
* prepare and separate material for further analysis, such as sample ionisation, chromatography, and electrophoresis 
* synthesise materials, such as epitaxy and continuous vapour deposition 
It also describes the instruments used in these experiments, such as mass spectrometers and chromatography columns and their outputs.

The OWL file is generated from the OBO file, but both can be edited in Protege (http://protege.stanford.edu/).

You can browse the ontology here: http://www.ebi.ac.uk/ols/ontologies/chmo

## Steps for release

1. You will need to obtain a tool to convert OBO to OWL (or _vice versa_ if you're editing the OWL), for example ROBOT, which is available here: http://robot.obolibrary.org/
2. `java -jar robot.jar convert --input rsc-cmo/chmo.obo --output rsc-cmo/chmo.owl`
3. Check that the resulting file doesn't violate DL: `java -jar robot.jar validate-profile --input rsc-cmo/chmo.owl --profile DL --output rsc-cmo/dl.txt`

Colin Batchelor

2019-08-16
