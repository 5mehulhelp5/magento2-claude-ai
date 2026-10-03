# Changelog

All notable changes to this extension are documented here. The format
is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/).

## [1.9.2] - 2026-10-03

### Fixed
- Dry Run Mode no longer creates checkpoints or folders. The update_config, set_store_logo and manage_products update actions now return the preview before any snapshot is taken.
- Store view and website scope writes from update_config and set_store_logo, and checkpoint restores of such values, are saved with the scope codes Magento reads (stores and websites), so the change now takes effect on the storefront.
- update_config action=read only returns values for paths on its allow-list, the same list that limits writes.
