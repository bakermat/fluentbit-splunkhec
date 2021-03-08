# Splunk HEC Example

This example showcases how to send logs & metrics to a Splunk Enterprise deployment via the Fluentd/Fluent Bit logging driver. Full documentation on the Splunk Fluent Bit output plugin can be found [here](https://docs.fluentbit.io/manual/pipeline/outputs/splunk).

The example runs as a Docker Compose deployment. This example uses Fluent Bit to send logs & metrics from containers directly to Splunk HEC. To learn more about HEC, visit [this guide](https://dev.splunk.com/enterprise/docs/dataapps/httpeventcollector/).

To deploy the example, check out this git repository, open a terminal and in this directory type:
```bash
$> docker-compose up --build -d
```

Splunk will become available on port 18000. You can login on [http://localhost:18000](http://localhost:18000) with `admin` and `changeme`.

Once logged in, visit the [search application](http://localhost:18000/en-US/app/search) to see the logs collected by Splunk.