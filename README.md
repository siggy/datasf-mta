# DataSF MTA

This repo contains notes on aggregating DataSF's `Municipal Transportation
Agency Board Resolutions` data set:
https://data.sfgov.org/City-Management-and-Ethics/Municipal-Transportation-Agency-Board-Resolutions/v5uc-gana

Socrata site:
https://dev.socrata.com/foundry/data.sfgov.org/v5uc-gana

## Retrieve full data set

Register an App Token at:
https://data.sfgov.org/profile/edit/developer_settings

```bash
curl -H "X-App-Token: $SFDATA_APP_TOKEN" "https://data.sfgov.org/resource/v5uc-gana.json?\$limit=10000&\$offset=0"
```

Example stored as (`v5uc-gana-10804.json`)

## Example agenda parsing

Item I on:
(https://www.sfmta.com/sites/default/files/reports-and-documents/2019/04/4-16-19_agenda_-_mtab.pdf)

Corresponds to:
(`4-16-19.yellow.meter`)
