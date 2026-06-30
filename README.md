The ontology is provided in two versions:

1. connection_pattern_DUL_DnS.ttl
   Full ontology including OWL axioms and SWRL rule templates.

2. connection_pattern_DUL_DnS_DL_only.ttl
   DL-only ontology used for OWL-DL consistency checking. SWRL rules were removed because the consistency check targets the OWL-DL axiomatization of the DUL/DnS alignment layer.

Consistency checking was performed using ROBOT with the HermiT reasoner:

java -Xmx6G -jar robot.jar reason --reasoner hermit --input connection_pattern_DUL_DnS_DL_only.ttl --dump-unsatisfiable unsat_hermit.ttl --output reasoned_hermit.ttl

The command completed successfully and produced reasoned_hermit.ttl. No inconsistency or unsatisfiable named classes were reported.
