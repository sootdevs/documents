This document serves to detail what data Sootbot, the Discord bot for the WilburSoot Discord server, and other related systems use while you are a member of the server.

We respect the privacy of your information. We fully understand how important privacy is, and thus we provide this document to support the protection of your privacy. This policy describes the types of information we may collect from you or that you may provide as a member of the WilburSoot Discord server via it's main bot, Sootbot.

This policy applies to information we collect via the Discord API and Sootbot, and no other data collection methods. Discord's privacy policy can be seen here: https://discord.com/privacy

Please note that we not knowingly log any data, personally identifiable or otherwise, for under 13s.

This document was inspired by Python Discord's privacy document, visible at https://pythondiscord.com/pages/privacy. Many features here are developed with him from their users and staff, so appreciation is necessary. Thank you, Python Discord!

The information we collect, how we collect it, and how it is stored:

  - Personally Identifiable Information:
    - We do not store any personally identifiable information unless it is required for moderation. This includes:
      - Message contents - if triggered by our anti-spam filters for example
      - Discord user data - username, ID, join date, created date.
      - Modmail - logs all messages to a secure database.

    - Sootbot logs all moderation actions into a PostgreSQL database stored securely and only directly accessible by 3 people, who are all trusted members of the server's staff team. This data may contain personally identifiable information.

    - Our Modmail system logs all messages sent to it in a secure logging system, along with other user data. This is only accessible by server staff, with the database only directly accessible by one person.

    - Data may be kept by the cache of the programming languages and services we use. This is not used for any purpose.

  - Non-personally identifable information:

    - Sootbot may use StatsD, a Python module for logging statisics, and Graphite, acting as a bridge for these statistics, for logging purposes. This data does not contain personally identifable information, and only ever stores a tally. It counts, for example, each message sent in the server. This data may be shown via the usage of a data dashboard such as Grafana. This does not store message content.

    - Sootbot may use Metricity, a Python program for logging statistics. This data does not contain personally identifable information unless provided by the user's set username, as it stores your username, ID, join date, created date and avatar hash. This program also may store message IDs, but does not store message content.

    - You can request to opt-out of the Metricity system if you do not wish to have your messages counted and your username saved. You can do this by running ^opt_out in #bot-spam. You can opt-in again by running ^opt_in in #bot-spam.

    - We stress that neither of these metric logging services, StatsD or Metricity, log your messages. Both of these metric logging services are hosted securely and privately, and are not accessible without authentication. Access is only given to trusted members of the server staff team. These are only used for analysis and statistical reasons.

Contact:

  - Any and all questions regarding this document and the policies within it can be sent to the Data Controller. This can be done through Discord at `pixelflow#2332` or by old-fashioned email at `dan@wilburdiscord.com`. A Subject Access Request can be sent to this email too, however at times we may require proof of ownership for the accounts you are requesting for.

Other services:
  - Any other services that collect data are either not managed by the Sootbot/WilburSoot team or will have their policy set out upon usage. An example of this is the Google Forms service, which we may use at times.
