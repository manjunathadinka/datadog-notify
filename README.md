# datadog-notify

A simple shell script for creating events in Datadog. A great companion to Monit or other ops tools where you may want things reporting.
Prerequisites

    Curl
    Datadog API Key

Setup

    Put the script somewhere you can execute it from
    Export the environment variable DATADOG_API_KEY into the environment the script will be run in
    Invoke it! datadog-notify 'Event Title' 'A short message' 'success' 'optional:tags key:value'
    Enjoy seeing your deployments, service restarts and other events along side your monitoring stats!

Arguements

    The title of the event
    The message for the event
    Optionally, the alert level. One of: error, warning, info or success. Assumed to be info if not provided
    Optionally, some tags in key1:value1 key2:value2 format
