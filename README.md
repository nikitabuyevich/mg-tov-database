![Logo of OSM](./logo.jpg)

# MapleGlobal/Tales of Victoria's Database &middot; [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](./LICENSE)

This MySQL dump contains the latest backup of when Tales of Victoria officially shut down on September 23rd, 2018. Tales of Victoria was the underground server of MapleGlobal.

Using this data, anyone can recreate all the accounts, characters, items, etc. of MapleGlobal/Tales of Victoria.

Any personally identifiable information has been stripped.

**If you're serious about migrating this data, contact [asdf.asdf.dev@gmail.com](mailto:asdf.asdf.dev@gmail.com) to request the original [BCrypted](https://en.wikipedia.org/wiki/Bcrypt) hashed passwords.**

## Notes

* Importing this data will create a new schema called `wvsbeta`.
* The `user_point_transactions` table is grouped by `userid` and summed on the `amount` and the `pointtype` to retrieve the available cash type for an account.
* You can reference the [WvsGlobal](https://github.com/diamondo25/WvsGlobal) project which MapleGlobal/Tales of Victoria were based on to understand how to utilize this schema. You can also [download the full MapleGlobal/Tales of Victoria SQL schema](https://github.com/diamondo25/WvsGlobal/blob/master/SQLs/wvsbeta_sql_compatible.sql).

## Getting Started

Simply import the [mg-tov_data.sql.gz](./mg-tov_data.sql.gz) file into your own MySQL instance.

If you're coming over from an Odin based server, you can reference the [WvsGlobal Merge Parser](http://gitlab.com/nikitabuyevich/wvsglobal-merge-parser) project to see an example of how to merge the MapleGlobal/Tales of Victoria database schema to an Odin based one.

### Prerequisites

* [MySQL - v5.7.x](https://www.mysql.com/) - A relational database management system.

## Authors

* **[MapleGlobal Creators](https://github.com/diamondo25/WvsGlobal#credits)**

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
