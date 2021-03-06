# Querying EIPs<a name="vpc_eip_0003"></a>

## Function<a name="section52618256"></a>

This API is used to query EIPs.

## URI<a name="section3802258"></a>

GET /v1/\{project\_id\}/publicips

Example:

```
GET https://{Endpoint}/v1/{project_id}/publicips?limit={limit}&marker={marker}
```

[Table 1](#table51200735)  describes the parameters.

**Table  1**  Parameter description

<a name="table51200735"></a>
<table><thead align="left"><tr id="row8909633"><th class="cellrowborder" valign="top" width="24.997500249975%" id="mcps1.2.5.1.1"><p id="p50591634"><a name="p50591634"></a><a name="p50591634"></a>Name</p>
</th>
<th class="cellrowborder" valign="top" width="24.62753724627537%" id="mcps1.2.5.1.2"><p id="p4281684"><a name="p4281684"></a><a name="p4281684"></a>Mandatory</p>
</th>
<th class="cellrowborder" valign="top" width="19.548045195480455%" id="mcps1.2.5.1.3"><p id="p2939873918724"><a name="p2939873918724"></a><a name="p2939873918724"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="30.826917308269174%" id="mcps1.2.5.1.4"><p id="p11272110"><a name="p11272110"></a><a name="p11272110"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row40625737"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.2.5.1.1 "><p id="p2350413"><a name="p2350413"></a><a name="p2350413"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="24.62753724627537%" headers="mcps1.2.5.1.2 "><p id="p56165728"><a name="p56165728"></a><a name="p56165728"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="19.548045195480455%" headers="mcps1.2.5.1.3 "><p id="p3248766718724"><a name="p3248766718724"></a><a name="p3248766718724"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.4 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>Specifies the project ID. </p>
</td>
</tr>
<tr id="row8409368"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.2.5.1.1 "><p id="p10070188"><a name="p10070188"></a><a name="p10070188"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="24.62753724627537%" headers="mcps1.2.5.1.2 "><p id="p10378893"><a name="p10378893"></a><a name="p10378893"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.548045195480455%" headers="mcps1.2.5.1.3 "><p id="p1425535118724"><a name="p1425535118724"></a><a name="p1425535118724"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.4 "><p id="p47529299"><a name="p47529299"></a><a name="p47529299"></a>Specifies the start resource ID of pagination query. If the parameter is left blank, only resources on the first page are queried.</p>
</td>
</tr>
<tr id="row25110514"><td class="cellrowborder" valign="top" width="24.997500249975%" headers="mcps1.2.5.1.1 "><p id="p20685786"><a name="p20685786"></a><a name="p20685786"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="24.62753724627537%" headers="mcps1.2.5.1.2 "><p id="p64935954"><a name="p64935954"></a><a name="p64935954"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="19.548045195480455%" headers="mcps1.2.5.1.3 "><p id="p1383277618724"><a name="p1383277618724"></a><a name="p1383277618724"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30.826917308269174%" headers="mcps1.2.5.1.4 "><a name="ul58841132132312"></a><a name="ul58841132132312"></a><ul id="ul58841132132312"><li>Specifies the number of records returned on each page.</li><li>The value ranges from 0 to intmax.</li></ul>
</td>
</tr>
</tbody>
</table>

## Request Message<a name="section34220326"></a>

-   Request parameter

    None

-   Example request

    None


## Response Message<a name="section39547486"></a>

-   Response parameter

    **Table  2**  Response parameter

    <a name="table22603002152149"></a>
    <table><thead align="left"><tr id="row30843029152149"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="p15257431152149"><a name="p15257431152149"></a><a name="p15257431152149"></a>Name</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="p44693705152149"><a name="p44693705152149"></a><a name="p44693705152149"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="p63420361152149"><a name="p63420361152149"></a><a name="p63420361152149"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row36775597152149"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="p26033374152149"><a name="p26033374152149"></a><a name="p26033374152149"></a>publicips</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="p746714339186"><a name="p746714339186"></a><a name="p746714339186"></a>Array of <a href="#table83964341880">publicips</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="p14951203152149"><a name="p14951203152149"></a><a name="p14951203152149"></a>Specifies the EIP objects. For details, see <a href="#table83964341880">Table 3</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **Table  3**  Description of the  **publicips**  field

    <a name="table83964341880"></a>
    <table><thead align="left"><tr id="row608739661880"><th class="cellrowborder" valign="top" width="36.046395360463954%" id="mcps1.2.4.1.1"><p id="p318442431880"><a name="p318442431880"></a><a name="p318442431880"></a>Name</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.90720927907209%" id="mcps1.2.4.1.2"><p id="p201897271880"><a name="p201897271880"></a><a name="p201897271880"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="36.046395360463954%" id="mcps1.2.4.1.3"><p id="p247551571880"><a name="p247551571880"></a><a name="p247551571880"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row590107001880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p151373871880"><a name="p151373871880"></a><a name="p151373871880"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p623914921880"><a name="p623914921880"></a><a name="p623914921880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p205460611880"><a name="p205460611880"></a><a name="p205460611880"></a>Specifies the unique identifier of the EIP.</p>
    </td>
    </tr>
    <tr id="row506968211880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p128018091880"><a name="p128018091880"></a><a name="p128018091880"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p394853281880"><a name="p394853281880"></a><a name="p394853281880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul263945115243"></a><a name="ul263945115243"></a><ul id="ul263945115243"><li>Specifies the EIP status.</li><li>Possible values are as follows:<a name="ul7905205815810"></a><a name="ul7905205815810"></a><ul id="ul7905205815810"><li><strong id="b84235270610153"><a name="b84235270610153"></a><a name="b84235270610153"></a>FREEZED</strong> (Frozen)</li><li><strong id="b842352706181622"><a name="b842352706181622"></a><a name="b842352706181622"></a>BIND_ERROR</strong> (Binding failed)</li><li><strong id="b842352706181646"><a name="b842352706181646"></a><a name="b842352706181646"></a>BINDING</strong> (Binding)</li><li><strong id="b84235270618176"><a name="b84235270618176"></a><a name="b84235270618176"></a>PENDING_DELETE</strong> (Releasing)</li><li><strong id="b842352706181716"><a name="b842352706181716"></a><a name="b842352706181716"></a>PENDING_CREATE</strong> (Assigning)</li><li><strong id="b842352706181818"><a name="b842352706181818"></a><a name="b842352706181818"></a>PENDING_UPDATE</strong> (Updating)</li><li><strong id="b842352706181834"><a name="b842352706181834"></a><a name="b842352706181834"></a>DOWN</strong> (Unbound)</li><li><strong id="b84235270610164"><a name="b84235270610164"></a><a name="b84235270610164"></a>ACTIVE</strong> (Bound)</li><li><strong id="b842352706181859"><a name="b842352706181859"></a><a name="b842352706181859"></a>ELB</strong> (Bound to a load balancer)</li><li><strong id="b842352706103022"><a name="b842352706103022"></a><a name="b842352706103022"></a>ERROR</strong> (Exceptions)</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row230260811880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p30749271"><a name="p30749271"></a><a name="p30749271"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p379401841880"><a name="p379401841880"></a><a name="p379401841880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul7176216121014"></a><a name="ul7176216121014"></a><ul id="ul7176216121014"><li>Specifies the EIP type.</li><li>Constraints:<a name="ul9738153015499"></a><a name="ul9738153015499"></a><ul id="ul9738153015499"><li>The configured value must be supported by the system. </li><li><strong id="b1696193019360"><a name="b1696193019360"></a><a name="b1696193019360"></a>publicip_id</strong> is an IPv4 port. If <strong id="b16961830153614"><a name="b16961830153614"></a><a name="b16961830153614"></a>publicip_type</strong> is not specified, the default value is <strong id="b1569714306364"><a name="b1569714306364"></a><a name="b1569714306364"></a>5_bgp</strong>.</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row389218135338"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p59108624"><a name="p59108624"></a><a name="p59108624"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p904808818330"><a name="p904808818330"></a><a name="p904808818330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p40237373"><a name="p40237373"></a><a name="p40237373"></a>Specifies the obtained EIP if only IPv4 EIPs are available. </p>
    </td>
    </tr>
    <tr id="row283940631880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p182177951880"><a name="p182177951880"></a><a name="p182177951880"></a>private_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p60695041880"><a name="p60695041880"></a><a name="p60695041880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul1693412582014"></a><a name="ul1693412582014"></a><ul id="ul1693412582014"><li>Specifies the private IP address bound with the EIP.</li><li>This parameter is returned only when a private IP address is bound with the EIP.</li></ul>
    </td>
    </tr>
    <tr id="row264614551880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p630030811880"><a name="p630030811880"></a><a name="p630030811880"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p397229231880"><a name="p397229231880"></a><a name="p397229231880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul420471472010"></a><a name="ul420471472010"></a><ul id="ul420471472010"><li>Specifies the port ID.</li><li>This parameter is returned only when a private IP address is bound with the EIP.</li></ul>
    </td>
    </tr>
    <tr id="row340905521880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p98713501880"><a name="p98713501880"></a><a name="p98713501880"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p58747301880"><a name="p58747301880"></a><a name="p58747301880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p19867509217"><a name="p19867509217"></a><a name="p19867509217"></a>Specifies the project ID.</p>
    </td>
    </tr>
    <tr id="row548200921880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p112424711880"><a name="p112424711880"></a><a name="p112424711880"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p92119381880"><a name="p92119381880"></a><a name="p92119381880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p36292894"><a name="p36292894"></a><a name="p36292894"></a>Specifies the time (UTC time) when the EIP was assigned.</p>
    </td>
    </tr>
    <tr id="row46164031880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p383843571880"><a name="p383843571880"></a><a name="p383843571880"></a>bandwidth_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p473107141880"><a name="p473107141880"></a><a name="p473107141880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p3934181618641"><a name="p3934181618641"></a><a name="p3934181618641"></a>Specifies the ID of the bandwidth associated with the EIP.</p>
    </td>
    </tr>
    <tr id="row626637421880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p425983371880"><a name="p425983371880"></a><a name="p425983371880"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p463832691880"><a name="p463832691880"></a><a name="p463832691880"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><p id="p2365466"><a name="p2365466"></a><a name="p2365466"></a>Specifies the bandwidth (Mbit/s).</p>
    </td>
    </tr>
    <tr id="row576448061880"><td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.1 "><p id="p387177161880"><a name="p387177161880"></a><a name="p387177161880"></a>bandwidth_share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.90720927907209%" headers="mcps1.2.4.1.2 "><p id="p21369006155933"><a name="p21369006155933"></a><a name="p21369006155933"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="36.046395360463954%" headers="mcps1.2.4.1.3 "><a name="ul2255712095"></a><a name="ul2255712095"></a><ul id="ul2255712095"><li>Specifies the EIP bandwidth type.</li><li>The value can be <strong id="b15499145815393"><a name="b15499145815393"></a><a name="b15499145815393"></a>PER</strong> or <strong id="b6500558143916"><a name="b6500558143916"></a><a name="b6500558143916"></a>WHOLE</strong>.<a name="ul729412507220"></a><a name="ul729412507220"></a><ul id="ul729412507220"><li><strong id="b16410175912395"><a name="b16410175912395"></a><a name="b16410175912395"></a>PER</strong>: Dedicated bandwidth</li><li><strong id="b114998124012"><a name="b114998124012"></a><a name="b114998124012"></a>WHOLE</strong>: Shared bandwidth</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   Example response

    ```
    {
        "publicips": [
            {
                "id": "6285e7be-fd9f-497c-bc2d-dd0bdea6efe0",
                "status": "DOWN",
                "type": "5_bgp",
                "public_ip_address": "161.xx.xx.9",
                "private_ip_address": "192.168.10.5",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "create_time": "2015-07-16 04:22:32",
                "bandwidth_id": "3fa5b383-5a73-4dcb-a314-c6128546d855",
                "bandwidth_share_type": "PER",
                "bandwidth_size": 5,
                
                "ip_version": 4
            },
            {
                "id": "80d5b82e-43b9-4f82-809a-37bec5793bd4",
                "status": "DOWN",
                "type": "5_bgp",
                "public_ip_address": "161.xx.xx.10",
                "private_ip_address": "192.168.10.6",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "create_time": "2015-07-16 04:23:03",
                "bandwidth_id": "a79fd11a-047b-4f5b-8f12-99c178cc780a",
                "bandwidth_share_type": "PER",
                "bandwidth_size": 5,
                
                "ip_version": 4
            }
        ]
    }
    ```


## Status Code<a name="section31981619"></a>

See  [Status Codes](status-codes.md).

## Error Code<a name="section85821649202813"></a>

See  [Error Codes](error-codes.md).

