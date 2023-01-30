# EspoCRM Nightly

Nightly builds are built automatically every day at 00:00 (UTC) from the files in the [EspoCRM repository](https://github.com/espocrm/espocrm) as they are.

## ⚠️ Disclaimer ⚠️

**This project is not associated with the EspoCRM project nor Letrium LTD. Espo CRM® is a registered trademark of Letrium LTD. Any use is for referential purposes only and does not indicate any sponsorship, endorsement, or affiliation between Letrium LTD.**

**Keep in mind: you are responsible for [making backups](https://docs.espocrm.com/administration/backup-and-restore) before upgrade. Builts may contain changes that would break your EspoCRM instance.**

**USE AT YOUR OWN RISK!**
---

## Install

### 1. Download EspoCRM-full.zip package

To get the latest package, follow the [link][latest-release].

### 2. Go to the official documentation

Now follow the same steps as in the official documentation, starting from step [2. Upload EspoCRM files to your server](https://docs.espocrm.com/administration/installation/#2-upload-espocrm-files-to-your-server).

## Upgrade

❗**IMPORTANT**❗

**Ensure you have the latest version of EspoCRM present. You can do it by running `php command.php upgrade`**.

You may either download an upgrade package [manually][latest-release], or use the following cURL or Wget command:

```sh
wget -q "https://github.com/arkadywtf/espocrm-nightly/releases/download/nightly-$(date +'%Y-%m-%d')/EspoCRM-upgrade.zip"
```

```sh
curl -sfLO "https://github.com/arkadywtf/espocrm-nightly/releases/download/nightly-$(date +'%Y-%m-%d')/EspoCRM-upgrade.zip"
```

### Upgrade from command line

Command to run:

```sh
php command.php upgrade -y --file="EspoCRM-upgrade.zip"
```

### Upgrade from UI

This is **not recommended way** to upgrade. If you wish to learn more, [visit the official documentation](https://docs.espocrm.com/administration/upgrading/#upgrade-from-ui).

## License

Licensed under [European Union Public License][eupl_url], version 1.2 or later, ([LICENSE](LICENSE) or https://joinup.ec.europa.eu/collection/eupl/eupl-text-11-12)

The EUPL is a copyleft, GPL-compatible license managed by the European Union, with legally-equal translated versions in all languages of the EU. See [this introduction](https://joinup.ec.europa.eu/collection/eupl/introduction-eupl-licence) for information about the purpose, objectives and translations of the license. See also the [license compatibility matrix](https://joinup.ec.europa.eu/collection/eupl/matrix-eupl-compatible-open-source-licences).

## Author Information

[arkadywtf][author_url]

[author_url]: https://github.com/arkadywtf
[latest-release]: https://github.com/arkadywtf/espocrm-nightly/releases/latest
[eupl_url]: https://joinup.ec.europa.eu/collection/eupl/eupl-text-11-12