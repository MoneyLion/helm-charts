# README

This repo is meant to be used as a place to store shared helm library charts that can be used in application charts to reduce code duplication.

## Usage

To add a new chart create a new folder under the `charts` folder and put your Chart files in it. For library charts, you should have a `Chart.yaml` and a `templates` folder containing all the templates. 

You can push the chart directly to the `main` branch, or if you don't have push permission, please create a PR and ask for a review from the SRE team. Once your code is merged to the main branch, a workflow will run to publish your chart and then you can use it as a dependency in your application chart.

You can refer to this [guide][1] on how to use a Helm library chart and we also have a [PoC][2] that you can refer to for how to use the template in your application chart.

[1]: https://helm.sh/docs/topics/library_charts/
[2]: https://github.com/MoneyLion/templateapi/blob/master/infra/charts/templateapi/templates/configmaptest.yaml
