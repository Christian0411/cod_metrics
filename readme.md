# cod_metrics 
Export CoD Warzone metrics into graphite!

## Usage

Get the ACT_SSO_COOKIE from my.callofduty.com:
- Login to http://my.callofduty.com
- Use the developer console to get the ACT_SSO_COOKIE

In the telegraf.conf file:
- Add your battle.net id by replaceing <battleid> with it. For the `#` use `%23`. So something like name%238723
- Add your ACT_SSO_COOKIE where it says <cookie>

Run `docker-compose up -d`

If everything worked you should see

See your grafana dashboard: https://localhost:3000

See https://www.linode.com/docs/uptime/monitoring/install-graphite-and-grafana/ for how to add graphite

## Metrics
Metrics are exported by flattening the response from the API JSON response  
