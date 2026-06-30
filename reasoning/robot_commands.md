# ROBOT/HermiT Reasoning Commands

This file records the commands used to check the DL-only version of the ontology.

Command:
java -Xmx6G -jar robot.jar reason --reasoner hermit --input ontology/connection_pattern_DUL_DnS_DL_only.ttl --dump-unsatisfiable reasoning/unsat_hermit.ttl --output ontology/reasoned_hermit.ttl

## Java Version

The reasoning check was performed using Java 17.

Command:

```cmd
java -version
openjdk version "17.0.19"
OpenJDK Runtime Environment Temurin-17.0.19+10
OpenJDK 64-Bit Server VM Temurin-17.0.19+10
