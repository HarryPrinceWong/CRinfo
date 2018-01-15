If you would like your clan family to be listed at http://cr-api.com/clans — you will need to send us your clan configuration in YAML. Read this guide thoroughly on how to configure it and then [open a new issue](https://github.com/cr-api/cr-api-ux/issues) with your configuration.

Please remember to escape your config as shown below with the three backticks. First to open it, and then to close it.

<img src="https://github.com/cr-api/cr-api-ux/blob/master/media/escape-yaml.png?raw=true" width="300" />


## Fields

This table shows what all those fields mean

| Field | Description |
| --- | --- |
| name | Name of the family. |
| key | Shortcut name. Used in the URL path. |
| color | Brand color. See below by acceptable colors. HEX is not supported yet, so use the closest match. |
| emblem | Clan Badge. Find it from your clan page or look up in [cr-api/cr-api-assets/badges](https://github.com/cr-api/cr-api-assets/tree/master/badges) |
| info | Optional information. Used in clans page. |
| clans | Name and tags of your clans. |
| sort | Sort order of the clans. Don’t include this field if you wish the clans be sorted according to the order in the `clans` field. Use `sort: trophy` if you want the clans to be sorted according to the clan score. |

### Info fields

| Field | Description |
| --- | --- |
| logo | Please provide URL to your logo and we will upload it. |
| description | Family description in markdown. Please be brief as it will push all your clans down if it is too long. |
| social | Links to social media sites. |

### Social Links

You may order these in any order. The site will display them according to the order that you have entered in your configuration.

- application: url
- discord: url
- email: mailto_url
- facebook: url
- instagram: url
- twitch: url
- twitter: url
- website: url
- youtube: url

### Clans

| Field | Description |
| --- | --- |
| name | Name of the clan |
| tag | Clan tag without the `#` symbol |


## Colors

[[https://github.com/cr-api/cr-api-docs/blob/master/docs/img/colors.png|alt=colors]]

## Examples

### Reddit Alpha Clan Family

http://cr-api.com/clan/family/racf/clans

```yaml
  - name: Reddit Alpha Clan Family
    key: racf
    color: red
    emblem: A_Char_Rocket_02
    info:
      logo: /static/img/brands/logo/racf.svg
      description: >
        The **Reddit Alpha Clan Family** (RACF) consists of 8 trophy-pushing clans.

        Our clan family is home to many of Clash Royale’s greatest tournament players,
        three of whom made it to the Crown Duel.
        We have 2 clans on the **global leaderboard** with **Reddit Alpha** consistently in the top 20
        and **Reddit Bravo** consistently in the top 200.
        Every clan in our family finishes the clan crown chest early every time.
      social:
        - twitter: http://twitter.com/RedditAlpha
        - discord: http://discord.gg/racf
        - twitch: https://www.twitch.tv/woody
        - reddit: http://www.reddit.com/r/CRRedditAlpha/
        - youtube: https://www.youtube.com/channel/UCjC5dP9z3XQY6OEPWh5RiLw
        - website: http://docs.redditalpha.com
    clans:
      - name: Reddit Alpha
        tag: 2CCCP
      - name: Reddit Bravo
        tag: 2U2GGQJ
      - name: Reddit Charlie
        tag: 2QUVVVP
      - name: Reddit Delta
        tag: Y8GYCGV
      - name: Reddit Echo
        tag: LGVV2CG
      - name: Reddit Foxtrot
        tag: QUYCYV8
      - name: Reddit Golf
        tag: GUYGVJY
      - name: Reddit Hotel
        tag: UGQ28YU
      - name: RACF Mini
        tag: 22LR8JJ2
      - name: RACF Mini2
        tag: 2Q09VJC8
```

### Nova eSports

http://cr-api.com/clan/family/nova/clans

```yaml
- name: Nova eSports
  key: nova
  color: purple
  emblem: Star_Shine_03
  sort: trophy
  info:
    logo: /static/img/brands/logo/nova.svg
    description: >
      **Competitive excellence through community-driven values.**
      Nova is a mobile-focused eSports organization committed to empowering
      individuals through a supportive team environment.
      We look for talent that has the character to back it up.
      That talent is cultivated and supported through team-based growth strategies and
      passionate staff that care about player outcomes.
      Community is the foundation of those outcomes and is the core of player dedication.
    social:
      - website: https://novaesports.com/
      - twitter: https://twitter.com/NovaeSportsTeam
      - instagram: https://instagram.com/novaesportsgg
      - facebook: https://facebook.com/OfficialNovaeSports
      - twitch: https://twitch.tv/NovaeSportsGG
      - youtube: https://www.youtube.com/channel/UC4JS5NiRp4Sy1wl6qFkW3GQ
      - application: https://novaesports.com/apply
      - email: mailto:pr@novaesports.com
  clans:
    - name: Nova eSports
      tag: LCVUYCR
    - name: Nova l Brazil
      tag: JVRPGV8
    - name: Nova l 大唐天子
      tag: RVL2PQQ
    - name: Nova l NA
      tag: 88UGGYG
    - name: Nova l Hispania
      tag: 2CQQVQCU
    - name: Nova l EG
      tag: 8YLJ8UL2
    - name: Nova l JPN
      tag: 2GYJL2GQ
    - name: Nova l Canada
      tag: 8PLYP8V
    - name: Nova Turkey
      tag: CYCJJLG
    - name: Nova l Swiss
      tag: 8RR89PUY
    - name: Nova FrenchArmy
      tag: 8VG2C9CJ
    - name: GloryMakersNova
      tag: 8R2C0G9Y
    - name: Gladiators™Nova
      tag: 82JRG0UV
```
