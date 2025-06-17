# Nova Value Widget

[![Latest Version on Packagist](https://img.shields.io/packagist/v/mlsolutions/value-widget)](https://packagist.org/packages/mlsolutions/value-widget)
[![Total Downloads](https://img.shields.io/packagist/dt/mlsolutions/value-widget)](https://packagist.org/packages/mlsolutions/value-widget)
[![License](https://img.shields.io/packagist/l/mlsolutions/value-widget)](https://github.com/ml-solutions-ltda/value-widget/blob/main/LICENSE)

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ml-solutions-ltda/value-widget/main/screenshots/dark.png">
  <img alt="Nova Welcome Card in Action" src="https://raw.githubusercontent.com/ml-solutions-ltda/value-widget/main/screenshots/light.png">
</picture>

A simple widget for laravel [Nova Dashboard](https://github.com/ml-solutions-ltda/nova-dashboard).

# Installation

You can install the package via composer:

```
composer require mlsolutions/value-widget
```

## Basic Usage

```php
use MlSolutions\NovaDashboard\Filters;
use MlSolutions\ValueWidget\ValueWidget;
use Laravel\Nova\Http\Requests\NovaRequest;

class MyWidget extends ValueWidget
{
    public function configure(NovaRequest $request): void
    {
        $this->icon('<svg></svg> or heroicons name');
        $this->title('My Widget');
        $this->textColor(dark: '#845adf', light: '#845adf');
        $this->backgroundColor('#845adf4f');
    }

    public function value(Filters $filters): mixed
    {
      //
    }
}
```

## ⭐️ Show Your Support

Please give a ⭐️ if this project helped you!

### Other Packages You Might Like

- [Nova Dashboard](https://github.com/ml-solutions-ltda/nova-dashboard) - The missing dashboard for Laravel Nova!
- [Nova Welcome Card](https://github.com/ml-solutions-ltda/nova-welcome-card) - A configurable version of the `Help card` that comes with Nova.
- [Icon Action Toolbar](https://github.com/ml-solutions-ltda/icon-action-toolbar) - Replaces the default boring action menu with an inline row of icon-based actions.
- [Expandable Table Row](https://github.com/ml-solutions-ltda/expandable-table-row) - Provides an easy way to append extra data to each row of your resource tables.
- [Collapsible Resource Manager](https://github.com/ml-solutions-ltda/collapsible-resource-manager) - Provides an easy way to order and group your resources on the sidebar.
- [Resource Navigation Tab](https://github.com/ml-solutions-ltda/resource-navigation-tab) - Organize your resource fields into tabs.
- [Resource Navigation Link](https://github.com/ml-solutions-ltda/resource-navigation-link) - Create links to internal or external resources.
- [Nova Mega Filter](https://github.com/ml-solutions-ltda/nova-mega-filter) - Display all your filters in a card instead of a tiny dropdown!
- [Nova Pill Filter](https://github.com/ml-solutions-ltda/nova-pill-filter) - A Laravel Nova filter that renders into clickable pills.
- [Nova Slider Filter](https://github.com/ml-solutions-ltda/nova-slider-filter) - A Laravel Nova filter for picking range between a min/max value.
- [Nova Range Input Filter](https://github.com/ml-solutions-ltda/nova-range-input-filter) - A Laravel Nova range input filter.
- [Nova FilePond](https://github.com/ml-solutions-ltda/nova-filepond) - A Nova field for uploading File, Image and Video using Filepond.
- [Custom Relationship Field](https://github.com/ml-solutions-ltda/custom-relationship-field) - Emulate HasMany relationship without having a real relationship set between resources.
- [Column Toggler](https://github.com/ml-solutions-ltda/column-toggler) - A Laravel Nova package that allows you to hide/show columns in the index view.
- [Batch Edit Toolbar](https://github.com/ml-solutions-ltda/batch-edit-toolbar) - Allows you to update a single column of a resource all at once directly from the index page.

## License

The MIT License (MIT). Please see [License File](https://raw.githubusercontent.com/ml-solutions-ltda/value-widget/main/LICENSE) for more information.
