# Querying a Host List<a name="EN-US_TOPIC_0172486227"></a>

## Function<a name="section389618791731"></a>

This API is used to query a host list of a specified cluster.

## URI<a name="section3064850017952"></a>

-   Format

    GET /v1.1/\{project\_id\}/clusters/\{cluster\_id\}/hosts

-   Parameter description

    **Table  1**  URI parameter description

    <a name="table49499141194754"></a>
    <table><thead align="left"><tr id="row33700024194754"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="p16571835194812"><a name="p16571835194812"></a><a name="p16571835194812"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.2"><p id="p141410194812"><a name="p141410194812"></a><a name="p141410194812"></a>Mandatory</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p11454278194812"><a name="p11454278194812"></a><a name="p11454278194812"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row6505449415356"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p3492262515356"><a name="p3492262515356"></a><a name="p3492262515356"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p1016041415356"><a name="p1016041415356"></a><a name="p1016041415356"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1768719515356"><a name="p1768719515356"></a><a name="p1768719515356"></a>Project ID. For details on how to obtain the project ID, see <a href="obtaining-a-project-id.md">Obtaining a Project ID</a>.</p>
    </td>
    </tr>
    <tr id="row37407495194754"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p56702435194812"><a name="p56702435194812"></a><a name="p56702435194812"></a>cluster_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p29494508194812"><a name="p29494508194812"></a><a name="p29494508194812"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p40820562194812"><a name="p40820562194812"></a><a name="p40820562194812"></a>Cluster ID</p>
    </td>
    </tr>
    </tbody>
    </table>


## Request<a name="section27807627171231"></a>

**Table  2**  Request parameter description

<a name="table32644073161516"></a>
<table><thead align="left"><tr id="row43445380161516"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p29414883161516"><a name="p29414883161516"></a><a name="p29414883161516"></a>Parameter</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.2"><p id="p33795347161516"><a name="p33795347161516"></a><a name="p33795347161516"></a>Mandatory</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.3"><p id="p7484174311367"><a name="p7484174311367"></a><a name="p7484174311367"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="45%" id="mcps1.2.5.1.4"><p id="p53068604161516"><a name="p53068604161516"></a><a name="p53068604161516"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row27166366161516"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p52992019161516"><a name="p52992019161516"></a><a name="p52992019161516"></a>pageSize</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="p64495161161516"><a name="p64495161161516"></a><a name="p64495161161516"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="p6484174315368"><a name="p6484174315368"></a><a name="p6484174315368"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="45%" headers="mcps1.2.5.1.4 "><p id="p56725559161516"><a name="p56725559161516"></a><a name="p56725559161516"></a>Maximum number of clusters displayed on a page</p>
<p id="p40767991161516"><a name="p40767991161516"></a><a name="p40767991161516"></a>Value range: [1-2147483646]. The default value is <strong id="b159151136204914"><a name="b159151136204914"></a><a name="b159151136204914"></a>10</strong>.</p>
</td>
</tr>
<tr id="row31367606161516"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p57748190161516"><a name="p57748190161516"></a><a name="p57748190161516"></a>currentPage</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="p47091798161516"><a name="p47091798161516"></a><a name="p47091798161516"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="p34851043113614"><a name="p34851043113614"></a><a name="p34851043113614"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="45%" headers="mcps1.2.5.1.4 "><p id="p56339270161516"><a name="p56339270161516"></a><a name="p56339270161516"></a>Current page number The default value is <strong id="b84235270615612"><a name="b84235270615612"></a><a name="b84235270615612"></a>1</strong>.</p>
</td>
</tr>
</tbody>
</table>

## Response<a name="section6047763217644"></a>

**Table  3**  Response parameter description

<a name="table62954996104116"></a>
<table><thead align="left"><tr id="row50672710104116"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="p10848813104116"><a name="p10848813104116"></a><a name="p10848813104116"></a><strong id="b1877515381938"><a name="b1877515381938"></a><a name="b1877515381938"></a>Parameter</strong></p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.2"><p id="p43671186104116"><a name="p43671186104116"></a><a name="p43671186104116"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p47705183104116"><a name="p47705183104116"></a><a name="p47705183104116"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row38914633104116"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p47671482104141"><a name="p47671482104141"></a><a name="p47671482104141"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p45292505104141"><a name="p45292505104141"></a><a name="p45292505104141"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p44814299104141"><a name="p44814299104141"></a><a name="p44814299104141"></a>Total number of hosts in a list</p>
</td>
</tr>
<tr id="row19491349104116"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p16863286104133"><a name="p16863286104133"></a><a name="p16863286104133"></a>hosts</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p54145644104133"><a name="p54145644104133"></a><a name="p54145644104133"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p159111050153212"><a name="p159111050153212"></a><a name="p159111050153212"></a>Host parameters</p>
<p id="p50701308104133"><a name="p50701308104133"></a><a name="p50701308104133"></a>For details, see <a href="#table21026630171650">Table 4</a>.</p>
</td>
</tr>
</tbody>
</table>

**Table  4** **Hosts**  parameter description

<a name="table21026630171650"></a>
<table><thead align="left"><tr id="row25475785171650"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="p31080335171739"><a name="p31080335171739"></a><a name="p31080335171739"></a><strong id="b15444141017516"><a name="b15444141017516"></a><a name="b15444141017516"></a>Parameter</strong></p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.2"><p id="p41349730171739"><a name="p41349730171739"></a><a name="p41349730171739"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.4.1.3"><p id="p60993867171739"><a name="p60993867171739"></a><a name="p60993867171739"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row64164652171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p29954363171650"><a name="p29954363171650"></a><a name="p29954363171650"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p35827707171650"><a name="p35827707171650"></a><a name="p35827707171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p16363131171650"><a name="p16363131171650"></a><a name="p16363131171650"></a>VM ID</p>
</td>
</tr>
<tr id="row13050456171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p50454016171650"><a name="p50454016171650"></a><a name="p50454016171650"></a>ip</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p47886046171650"><a name="p47886046171650"></a><a name="p47886046171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p53564516171650"><a name="p53564516171650"></a><a name="p53564516171650"></a>VM IP address</p>
</td>
</tr>
<tr id="row12318597171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p58282272171650"><a name="p58282272171650"></a><a name="p58282272171650"></a>flavor</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p3683120171650"><a name="p3683120171650"></a><a name="p3683120171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p29897333171650"><a name="p29897333171650"></a><a name="p29897333171650"></a>VM flavor ID</p>
</td>
</tr>
<tr id="row640547171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p51884380171650"><a name="p51884380171650"></a><a name="p51884380171650"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p37262675171650"><a name="p37262675171650"></a><a name="p37262675171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p1112113610339"><a name="p1112113610339"></a><a name="p1112113610339"></a>VM type</p>
<p id="p65486689171650"><a name="p65486689171650"></a><a name="p65486689171650"></a>Currently, MasterNode, CoreNode, and TaskNode are supported.</p>
</td>
</tr>
<tr id="row52509293171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p25394365171650"><a name="p25394365171650"></a><a name="p25394365171650"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p48232943171650"><a name="p48232943171650"></a><a name="p48232943171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p14554272171650"><a name="p14554272171650"></a><a name="p14554272171650"></a>VM name</p>
</td>
</tr>
<tr id="row63879587171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p6864084171650"><a name="p6864084171650"></a><a name="p6864084171650"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p5213748171650"><a name="p5213748171650"></a><a name="p5213748171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p19660467171650"><a name="p19660467171650"></a><a name="p19660467171650"></a>Current VM state</p>
</td>
</tr>
<tr id="row42726478171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p38292731171650"><a name="p38292731171650"></a><a name="p38292731171650"></a>mem</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p50132509171650"><a name="p50132509171650"></a><a name="p50132509171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p34201443171650"><a name="p34201443171650"></a><a name="p34201443171650"></a>Memory</p>
</td>
</tr>
<tr id="row39377536171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p35463825171650"><a name="p35463825171650"></a><a name="p35463825171650"></a>cpu</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p11730090171650"><a name="p11730090171650"></a><a name="p11730090171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p10613249171650"><a name="p10613249171650"></a><a name="p10613249171650"></a>Number of CPU cores</p>
</td>
</tr>
<tr id="row28410384171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p19539777171650"><a name="p19539777171650"></a><a name="p19539777171650"></a>root_volume_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p22550052171650"><a name="p22550052171650"></a><a name="p22550052171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p14614951171650"><a name="p14614951171650"></a><a name="p14614951171650"></a>OS disk capacity</p>
</td>
</tr>
<tr id="row64425697171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p51098939171650"><a name="p51098939171650"></a><a name="p51098939171650"></a>data_volume_type</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p51364957171650"><a name="p51364957171650"></a><a name="p51364957171650"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p66920820171650"><a name="p66920820171650"></a><a name="p66920820171650"></a>Data disk type</p>
</td>
</tr>
<tr id="row65416474171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p64243064171650"><a name="p64243064171650"></a><a name="p64243064171650"></a>data_volume_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p55078124171650"><a name="p55078124171650"></a><a name="p55078124171650"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p32143059171650"><a name="p32143059171650"></a><a name="p32143059171650"></a>Data disk capacity</p>
</td>
</tr>
<tr id="row20852078171650"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="p11296761171650"><a name="p11296761171650"></a><a name="p11296761171650"></a>data_volume_count</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.2 "><p id="p29864308171650"><a name="p29864308171650"></a><a name="p29864308171650"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.4.1.3 "><p id="p3089844171650"><a name="p3089844171650"></a><a name="p3089844171650"></a>Number of data disks</p>
</td>
</tr>
</tbody>
</table>

## Example<a name="section107789113217"></a>

-   Example request

    None

-   Example response

    ```
    {
      "total": 5,
      "hosts": [
        {
          "id": "063d1d47-ae91-4a48-840c-b3cfe4efbcf0",
          "name": "a78e161c-d14f-4b68-8c2d-0219920ce844_node_core_IQhiC",
          "ip": "192.168.0.169",
          "status": "ACTIVE",
          "flavor": "c2.2xlarge.linux.mrs",
          "type": "Core",
          "mem": "16384",
          "cpu": "8",
          "root_volume_size": "40",
          "data_volume_type": "SATA",
          "data_volume_size": 100,
          "data_volume_count": 1
        },
        {
          "id": "dc5c6208-faa2-4727-a65a-2b1ce235d350",
          "name": "a78e161c-d14f-4b68-8c2d-0219920ce844_node_master1_ASzkl",
          "ip": "192.168.0.156",
          "status": "ACTIVE",
          "flavor": "c2.4xlarge.linux.mrs",
          "type": "Master",
          "mem": "32768",
          "cpu": "16",
          "root_volume_size": "40",
          "data_volume_type": "SATA",
          "data_volume_size": 100,
          "data_volume_count": 1
        },
        {
          "id": "c0ce793d-848b-448a-835b-ea0cac534b09",
          "name": "a78e161c-d14f-4b68-8c2d-0219920ce844_node_core_ANnRN",
          "ip": "192.168.0.243",
          "status": "ACTIVE",
          "flavor": "c2.2xlarge.linux.mrs",
          "type": "Core",
          "mem": "16384",
          "cpu": "8",
          "root_volume_size": "40",
          "data_volume_type": "SATA",
          "data_volume_size": 100,
          "data_volume_count": 1
        },
        {
          "id": "95c23e43-ef6e-4732-b6ed-a5f1c7779fae",
          "name": "a78e161c-d14f-4b68-8c2d-0219920ce844_node_core_uRRiA",
          "ip": "192.168.0.126",
          "status": "ACTIVE",
          "flavor": "c2.2xlarge.linux.mrs",
          "type": "Core",
          "mem": "16384",
          "cpu": "8",
          "root_volume_size": "40",
          "data_volume_type": "SATA",
          "data_volume_size": 100,
          "data_volume_count": 1
        },
        {
          "id": "63bdbf75-1133-4a94-8c27-1fa12c8b9e70",
          "name": "a78e161c-d14f-4b68-8c2d-0219920ce844_node_master2_StqFu",
          "ip": "192.168.0.22",
          "status": "ACTIVE",
          "flavor": "c2.4xlarge.linux.mrs",
          "type": "Master",
          "mem": "32768",
          "cpu": "16",
          "root_volume_size": "40",
          "data_volume_type": "SATA",
          "data_volume_size": 100,
          "data_volume_count": 1
        }
      ]
    }
    ```


## Status Code<a name="section31921280171927"></a>

[Table 5](#table33682380171927)  describes the status code of this API.

**Table  5**  Status code

<a name="table33682380171927"></a>
<table><thead align="left"><tr id="row56379034171927"><th class="cellrowborder" valign="top" width="30%" id="mcps1.2.3.1.1"><p id="p28423228171927"><a name="p28423228171927"></a><a name="p28423228171927"></a>Status Code</p>
</th>
<th class="cellrowborder" valign="top" width="70%" id="mcps1.2.3.1.2"><p id="p20580145171927"><a name="p20580145171927"></a><a name="p20580145171927"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row35948064171927"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.3.1.1 "><p id="p3299040171927"><a name="p3299040171927"></a><a name="p3299040171927"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="70%" headers="mcps1.2.3.1.2 "><p id="p65895658171927"><a name="p65895658171927"></a><a name="p65895658171927"></a>The host list information has been successfully queried.</p>
</td>
</tr>
</tbody>
</table>

For the description about error status codes, see  [Status Codes](status-codes.md).

