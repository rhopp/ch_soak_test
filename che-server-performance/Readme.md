# Soak test for che.
Right now, there is only one scenario, which runs by default only once.

1) Create workspace
2) Start that workspace
3) Wait for it to be running
4) Delete that workspace
5) Repeat from step 1)

If you want to run it multiple times, edit src/test/resources/scenarios/my_perfcake_scenario.xml. Search for tag "run" and edit it's  value.

# How to run

1) `mvn clean install -DcheStarterHost=<cheStarterHost> -Dtoken=<token>`

That's it.

## Properties

_cheStarterHost_ - URL of che starter. For local cheStarter it is `http://localhost:10000`

_token_ - User token obtained from openshift.io

