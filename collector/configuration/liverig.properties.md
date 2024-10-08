# liverig.properties

<table data-full-width="true">
    <thead>
        <tr>
            <th width="429">Property</th>
            <th width="130" align="center">Type</th>
            <th width="238">Default</th>
            <th width="88" align="center">Since</th>
            <th align="center">UOM</th>
            <th>Valid Values</th>
            <th>Requires Property</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><code>data_path</code><br>Root directory, where to look for the configuration (<code>/conf</code>) and
                where collected data will be written (<code>/data</code>).</td>
            <td align="center"><code>string</code></td>
            <td><code>/opt/intelie/liverig</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_send_to_live</code><br>Whether to send collected data to Intelie Live (when true) or save
                it locally only, for example on protocol conversion mode.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>true</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_webapp</code><br>Enables the web application provision.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.hostname</code><br>Live access' hostname.</td>
            <td align="center"><code>string</code></td>
            <td><code>localhost</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.port</code><br>Live access' port.</td>
            <td align="center"><code>int</code></td>
            <td><code>5034</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.username</code><br>This collector's username to connect to Live.</td>
            <td align="center"><code>string</code></td>
            <td><code>live</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.password</code><br>This collector's password to connect to Live.</td>
            <td align="center"><code>string</code></td>
            <td></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.ssl.enable</code><br>Enables SSL connection to Live.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.17.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.ssl.fingerprints</code><br>SSL key fingerprints required for an SSL connection to Live.</td>
            <td align="center"><code>string[]</code></td>
            <td></td>
            <td align="center">2.17.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.backup.hostname</code><br>Backup Live (secondary Live client) access' hostname.</td>
            <td align="center"><code>string</code></td>
            <td></td>
            <td align="center">5.20.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.backup.port</code><br>Backup Live (secondary Live client used when main client is off)
                access' port.</td>
            <td align="center"><code>int</code></td>
            <td><code>0</code></td>
            <td align="center">5.20.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.backup.username</code><br>This collector's username to connect to secondary Live (used when
                main client is off).</td>
            <td align="center"><code>string</code></td>
            <td><code>live</code></td>
            <td align="center">5.20.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.backup.password</code><br>This collector's password to connect to secondary Live (used when
                main client is off).</td>
            <td align="center"><code>string</code></td>
            <td></td>
            <td align="center">5.20.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>live.backup.change.delay</code><br>Delay (in milliseconds) to switch the events destination to
                backup Live.</td>
            <td align="center"><code>long</code></td>
            <td><code>60000</code></td>
            <td align="center">5.20.0</td>
            <td align="center">ms</td>
            <td></td>
            <td><code>live.backup.hostname</code></td>
        </tr>
        <tr>
            <td><code>live.main.change.delay</code><br>Delay (in milliseconds) to switch the events destination to main
                Live.</td>
            <td align="center"><code>long</code></td>
            <td><code>60000</code></td>
            <td align="center">5.20.0</td>
            <td align="center">ms</td>
            <td></td>
            <td><code>live.backup.hostname</code></td>
        </tr>
        <tr>
            <td><code>connect_timeout</code><br>The connection timeout.</td>
            <td align="center"><code>long</code></td>
            <td><code>30000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>reconnect_minimum_delay</code><br>The minimum delay allowed on reconnections.</td>
            <td align="center"><code>long</code></td>
            <td><code>1000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>reconnect_maximum_delay</code><br>The maximum delay allowed on reconnections.</td>
            <td align="center"><code>long</code></td>
            <td><code>60000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>compression</code><br>Enables data compression with <em>zlib</em>. Modified during hello
                negotiation.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>true</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>request_threads</code><br>Maximum number of threads allowed to retrieve data.</td>
            <td align="center"><code>int</code></td>
            <td><code>64</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>hello_timeout</code><br>How much can the connection wait before the source hello is received.</td>
            <td align="center"><code>long</code></td>
            <td><code>10000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>idle_timeout</code><br>How much can the connection be idle before sending a keep-alive ping.</td>
            <td align="center"><code>long</code></td>
            <td><code>60000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>keep_alive_timeout</code><br>How much can the connection wait before the answer to a keep-alive
                ping.</td>
            <td align="center"><code>long</code></td>
            <td><code>10000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>resend_request_queue_capacity</code><br>Determines the length of a connection's resend request
                processing queue.</td>
            <td align="center"><code>int</code></td>
            <td><code>16</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>resend_rate</code><br>The default resend rate value is a good one when running at the rig site.
                When collecting from many sources at once, this value should be increased.</td>
            <td align="center"><code>long</code></td>
            <td><code>1000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">bytes/sec</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_realtime</code><br>Enables real time sync data.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>true</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>realtime_fetch_limit</code><br>Maximum time to fetch behind events when working in real time.</td>
            <td align="center"><code>long</code></td>
            <td><code>900000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td><code>enable_realtime</code></td>
        </tr>
        <tr>
            <td><code>realtime_fetch_tolerance</code><br>Maximum time to fetch forward events when working in real time.
            </td>
            <td align="center"><code>long</code></td>
            <td><code>900000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td><code>enable_realtime</code></td>
        </tr>
        <tr>
            <td><code>enable_backlog</code><br>Enables history data gathering.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>backlog_fetch_limit</code><br>The maximum time allowed to retrieve data when backlog enabled.</td>
            <td align="center"><code>long</code></td>
            <td><code>86400000</code></td>
            <td align="center">1.9.3</td>
            <td align="center">ms</td>
            <td></td>
            <td><code>enable_backlog</code></td>
        </tr>
        <tr>
            <td><code>enable_backlog_history</code><br>Enables the feature to retrieve backlog data within a start and
                end date.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.14.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>history_execution_period</code><br>The period factor that the backlog history will retrieve data.
            </td>
            <td align="center"><code>long</code></td>
            <td><code>1</code></td>
            <td align="center">2.14.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>enable_backlog_history</code></td>
        </tr>
        <tr>
            <td><code>backlog_history_fetch_limit</code><br>When backlog history is requested, this is the maximum fetch
                limit to retrieve by every <em>history_execution_period</em>.</td>
            <td align="center"><code>long</code></td>
            <td><code>900000</code></td>
            <td align="center">2.14.0</td>
            <td align="center">ms</td>
            <td></td>
            <td><code>enable_backlog_history</code></td>
        </tr>
        <tr>
            <td><code>backlog_history_depth_fetch_limit_in_meters</code><br>When backlog history is requested, this is
                the maximum fetch limit in depth meters to retrieve.</td>
            <td align="center"><code>long</code></td>
            <td><code>100</code></td>
            <td align="center">4.6.0</td>
            <td align="center">m</td>
            <td></td>
            <td><code>enable_backlog_history</code></td>
        </tr>
        <tr>
            <td><code>backlog_history_remote_execution_period_in_seconds</code><br>When backlog history is configured,
                this is the execution period to execute the request.</td>
            <td align="center"><code>long</code></td>
            <td><code>300</code></td>
            <td align="center">2.26.0</td>
            <td align="center">s</td>
            <td></td>
            <td><code>enable_backlog_history</code></td>
        </tr>
        <tr>
            <td><code>enable_remote_control_backlog_sync</code><br>Enables remote control for the backlog sync
                functionalities.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.26.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_remote_control</code><br>Enables remote control for the collector's functionalities.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.18.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>remote_control_max_threads</code><br>Maximum number of threads allowed for the remote-control
                functionalities.</td>
            <td align="center"><code>int</code></td>
            <td><code>4</code></td>
            <td align="center">2.18.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>enable_remote_control</code></td>
        </tr>
        <tr>
            <td><code>remote_control_queue_size</code><br>Maximum queue of remote-control requests.</td>
            <td align="center"><code>int</code></td>
            <td><code>128</code></td>
            <td align="center">2.18.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>enable_remote_control</code></td>
        </tr>
        <tr>
            <td><code>http_dump</code><br>Enables dumping http requests to the standard output.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>timestamp_adjustment_alpha</code><br>Timestamp adjustment factor to compensate the difference
                between the real-world time and the source's clock.</td>
            <td align="center"><code>double</code></td>
            <td><code>0.01</code></td>
            <td align="center">1.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>timestamp_adjustment_limit</code><br>The maximum difference allowed between the adjusted timestamp
                and the original one.</td>
            <td align="center"><code>double</code></td>
            <td><code>null</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>time_travel</code><br>This sets an offset time on the collector's clock.</td>
            <td align="center"><code>long</code></td>
            <td><code>0</code></td>
            <td align="center">1.6.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_lcd</code><br>Enables the collector to display its status on an LCD screen.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>true</code></td>
            <td align="center">2.7.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>lcd_type</code><br>The LCD's messaging type.</td>
            <td align="center"><code>string</code></td>
            <td><code>ipmi</code></td>
            <td align="center">2.7.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>enable_lcd</code></td>
        </tr>
        <tr>
            <td><code>crystalfontz_port</code><br>If the <em>lcd_type</em> is <strong>crystalfontz</strong>, this will
                set the port to access it.</td>
            <td align="center"><code>string</code></td>
            <td><code>/dev/ttyLCD</code></td>
            <td align="center">2.7.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>lcd_type</code></td>
        </tr>
        <tr>
            <td><code>crystalfontz_baud</code><br>If the <em>lcd_type</em> is <strong>crystalfontz</strong>, this will
                set its baud rate.</td>
            <td align="center"><code>string</code></td>
            <td><code>115200</code></td>
            <td align="center">2.7.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>lcd_type</code></td>
        </tr>
        <tr>
            <td><code>witsml_connect_timeout</code><br>The connection timeout value for a WITSML source.</td>
            <td align="center"><code>int</code></td>
            <td><code>15000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_request_timeout</code><br>The request timeout value for a WITSML source.</td>
            <td align="center"><code>int</code></td>
            <td><code>120000</code></td>
            <td align="center">1.0.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_query_force_return_elements_all</code><br>Enables forcing WITSML's <em>getFromStore</em> to
                return all elements.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">1.4.1</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml.certificates</code><br>Base directory where the HTTPS certificates are stored for WITSML
                client source configuration. <strong>This is not mandatory</strong>.</td>
            <td align="center"><code>string</code></td>
            <td><code>/opt/intelie/liverig/conf</code>/<code>witsml</code></td>
            <td align="center">4.7.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml.keystore</code><br>File name for the client keystore containing client private key and
                certificate for HTTPS certificate-based authentications for WITSML client sources.</td>
            <td align="center"><code>string</code></td>
            <td><code>witsml.jks</code></td>
            <td align="center">4.7.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml.keypass</code><br>Password for the client keystore.</td>
            <td align="center"><code>string</code></td>
            <td><code>liverig</code></td>
            <td align="center">4.7.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml.truststore</code><br>File name of the trusted WITSML servers store file. This file should
                contain the certificates the client can trust.<br>To disable the validation of server certificates, set
                the property <em>ignore_invalid_witsml_certificate</em> to <strong>true</strong>.</td>
            <td align="center"><code>string</code></td>
            <td><code>witsml-trust.jks</code></td>
            <td align="center">4.7.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml.trustpass</code><br>Password for the trusted servers keystore.</td>
            <td align="center"><code>string</code></td>
            <td><code>liverig</code></td>
            <td align="center">4.7.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>ignore_invalid_witsml_certificate</code><br>Enables ignoring invalid certificates from WITSML
                servers.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.19.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>opcua.applicationuri</code><br>The OPC-UA source's server application URI.</td>
            <td align="center"><code>string</code></td>
            <td><code>null</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>opcua.securitymode.min</code><br>The minimum endpoint security level required for the collector to
                try to connect to the OPC-UA server.</td>
            <td align="center"><code>string</code></td>
            <td><code>Sign</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td><code>None</code>, <code>Sign</code> or <code>SignAndEncrypt</code></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.securitymode.max</code><br>The minimum endpoint security level required for the collector to
                try to connect to the OPC-UA server.</td>
            <td align="center"><code>string</code></td>
            <td></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td><code>None</code>, <code>Sign</code> or <code>SignAndEncrypt</code></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.securitypolicy.min</code><br>The minimum endpoint security policy required by the collector
                to try to connect to the OPC-UA server.</td>
            <td align="center"><code>string</code></td>
            <td><code>Basic256Sha256</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td><code>None</code>, <code>Basic128Rsa15</code>, <code>Basic256</code>, <code>Basic256Sha256</code>,
                <code>Aes128_Sha256_RsaOaep</code> or <code>Aes256_Sha256_RsaPss</code></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.securitypolicy.max</code><br>The maximum endpoint security policy required by the collector
                to try to connect to the OPC-UA server.</td>
            <td align="center"><code>string</code></td>
            <td></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td><code>None</code>, <code>Basic128Rsa15</code>, <code>Basic256</code>, <code>Basic256Sha256</code>,
                <code>Aes128_Sha256_RsaOaep</code> or <code>Aes256_Sha256_RsaPss</code></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.certificates</code><br>Base directory for the OPC-UA certificates.</td>
            <td align="center"><code>string</code></td>
            <td><code>opcua</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.keystore</code><br>Name of the OPC-UA key store.</td>
            <td align="center"><code>string</code></td>
            <td><code>opcua.jks</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.storetype</code><br>OPC-UA Keystore Type</td>
            <td align="center"><code>string</code></td>
            <td><code>PKCS12</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.storepass</code><br>OPC-UA Keystore password</td>
            <td align="center"><code>string</code></td>
            <td><code>liverig</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.keyalias</code><br>OPC-UA's private key alias.</td>
            <td align="center"><code>string</code></td>
            <td><code>opcua</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.keypass</code><br>OPC-UA's private key password.</td>
            <td align="center"><code>string</code></td>
            <td><code>liverig</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>opcua.queuesize</code><br>Sets the OPC-UA's subscription queue size.</td>
            <td align="center"><code>int</code></td>
            <td><code>10</code></td>
            <td align="center">2.12.0</td>
            <td align="center"></td>
            <td></td>
            <td><code>opcua.applicationuri</code></td>
        </tr>
        <tr>
            <td><code>ignore_invalid_opc_certificate</code><br>Enables ignoring invalid certificates from OPC-UA and
                OPC-DA servers.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.23.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_witsml_tree_event</code><br><strong>This Property was removed on Liverig 2.22.0</strong>
            </td>
            <td align="center"><code>boolean</code></td>
            <td><code>true</code></td>
            <td align="center">2.17.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_tree_event_period_seconds</code><br><strong>This Property was removed on Liverig
                    2.22.0</strong></td>
            <td align="center"><code>long</code></td>
            <td><code>600</code></td>
            <td align="center">2.17.0</td>
            <td align="center">s</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>wildcard_period_in_seconds</code><br>Sets the Wildcard Period if the Request does not contain it.
            </td>
            <td align="center"><code>int</code></td>
            <td><code>600</code></td>
            <td align="center">2.22.0</td>
            <td align="center">s</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_change_mechanism_feature</code><br>Enables a mechanism for identifying change for data
                objects in a WITSML server</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">5.17.x</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_change_mechanism_delay_period_in_seconds</code><br>The number of seconds for the client to
                detect a change in a growing data object.</td>
            <td align="center"><code>int</code></td>
            <td><code>0</code></td>
            <td align="center">5.17.x</td>
            <td align="center">s</td>
            <td><code>witsml_change_mechanism_feature</code> = true</td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_change_mechanism_detection_period_in_seconds</code><br>The number of seconds for the client
                delayed to start</td>
            <td align="center"><code>int</code></td>
            <td><code>10</code></td>
            <td align="center">5.17.x</td>
            <td align="center">s</td>
            <td><code>witsml_change_mechanism_feature</code> = true</td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_change_mechanism_initial_last_change_feature</code><br>Enables the use of a default initial
                lastChange when starts the feature</td>
            <td align="center"><code>boolean</code></td>
            <td><code>true</code></td>
            <td align="center">5.17.x</td>
            <td align="center"></td>
            <td><code>witsml_change_mechanism_feature</code> = true</td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_change_mechanism_late_channels_feature</code><br>Allows to collect channels that arrive
                with low-frequency samples</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">5.17.x</td>
            <td align="center"></td>
            <td><code>witsml_change_mechanism_feature</code> = true</td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_change_mechanism_object_growing_feature</code><br>Enables the use of object-growing queries
                when there aren't changed objects</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">5.17.x</td>
            <td align="center"></td>
            <td><code>witsml_change_mechanism_feature</code> = true</td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_change_mechanism_initial_last_change_in_minutes</code><br>The number of minutes before now
                for use as the default last change for an initial request</td>
            <td align="center"><code>int</code></td>
            <td><code>1440</code></td>
            <td align="center">5.17.x</td>
            <td align="center">minutes</td>
            <td><code>witsml_change_mechanism_feature</code> = true</td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_revision</code></td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.24.1</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_revision_offset</code></td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">2.25.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>log_rotate_hour</code><br>Sets the hour of day to rotate Event logs.</td>
            <td align="center"><code>int</code></td>
            <td><code>4</code></td>
            <td align="center">2.18.1</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>minimum_diskspace_in_megabytes</code><br>Minimum available disk space required to collector work
                properly. The collector is restarted whenever the available disk space is less than the minimum
                required.</td>
            <td align="center"><code>int</code></td>
            <td><code>20</code></td>
            <td align="center">2.24.0</td>
            <td align="center">MB</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>internal_events_period_in_seconds</code><br>Period to compute and transmit the internal events
                reporting actual source configuration and basic server statistics to central sites.</td>
            <td align="center"><code>int</code></td>
            <td><code>60</code></td>
            <td align="center">4.7.0</td>
            <td align="center">s</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>internal_events_initial_delay_in_seconds</code><br>The initial delay for the computation and
                transmission of internal events can be customized freely.</td>
            <td align="center"><code>int</code></td>
            <td><code>60</code></td>
            <td align="center">4.7.0</td>
            <td align="center">s</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>enable_config_only_on_first_internal</code><br>Enables sending the internals
                <em>configurationStatus</em> field only on the first internal event sent.<br>The
                <em>configurationStatus</em> field contains a HashCode representation of every configuration file from
                the Liverig Collector, reducing bandwidth consumption for collector remote control features.</td>
            <td align="center"><code>boolean</code></td>
            <td><code>false</code></td>
            <td align="center">5.0.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>serial_connect_timeout</code><br>How much can the connection wait before retrying in case of
                failure when using a Serial Port.<br>The amount of time waiting is proportional to the number of failed
                attempts and it is given by <em>serial_connect_timeout</em> multiplied by the minimum between amount of
                attempts failed and <em>serial_max_retry_jump</em>.</td>
            <td align="center"><code>int</code></td>
            <td><code>15000</code></td>
            <td align="center">4.7.1</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>serial_max_retry_jump</code><br>The maximum serial timeout connection multiplier.</td>
            <td align="center"><code>int</code></td>
            <td><code>8</code></td>
            <td align="center">4.7.1</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_tree_request_feature</code><br>Enables the WITSML tree request feature to load WITSML objects to be used in Collector's Backlog Sync and Collector's Object Explorer screens</td>
            <td align="center"><code>boolean</code></td>
            <td><code>true</code></td>
            <td align="center">5.9.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_tree_request_object_limit</code><br>Maximum number of objects loaded in witsml tree.</td>
            <td align="center"><code>int</code></td>
            <td><code>1000</code></td>
            <td align="center">5.9.0</td>
            <td align="center"></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_tree_request_delay_time</code><br>Initial delay for search/pooling new objects.</td>
            <td align="center"><code>int</code></td>
            <td><code>0</code></td>
            <td align="center">5.9.0</td>
            <td align="center">ms</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td><code>witsml_tree_request_update_time</code><br>Time schedule for search/pooling new objects.</td>
            <td align="center"><code>int</code></td>
            <td><code>60</code></td>
            <td align="center">5.9.0</td>
            <td align="center">s</td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>

### Example

```
data_path=/opt/intelie/liverig

# if false, write output to local files in /opt/intelie/liverig/data
enable_send_to_live=true
# if true, enable local webapp for management; change the password in the login.properties file before enabling
enable_webapp=true
enable_remote_control=false

live.hostname=localhost
live.port=5034
live.username=live
live.password=

# Please copy the public key fingerprint from liverig-server to live.ssl.fingerprints below
live.ssl.enable=true
live.ssl.fingerprints=

connect_timeout=30000
reconnect_minimum_delay=1000
reconnect_maximum_delay=60000

compression=true
hello_timeout=10000
idle_timeout=60000
keep_alive_timeout=10000
resend_request_queue_capacity=16
resend_rate=1000
request_threads=64
http_dump=false

enable_realtime=true
# maximum ms to fetch behind when real time
realtime_fetch_limit=900000

enable_backlog=true

# Timestamp adjustment EWMA filter alpha value
#timestamp_adjustment_alpha=0.01
# Timestamp adjustment limit in ms (default value 2 * realtime_fetch_limit)
#timestamp_adjustment_limit=1800000

witsml_connect_timeout=15000
witsml_request_timeout=120000
wildcard_period_in_seconds=600

# LCD report via IPMI or Crystalfontz
#
# enable_lcd=true
# lcd_type=ipmi
# lcd_type=crystalfontz
# crystalfontz_port=/dev/ttyLCD
# crystalfontz_baud=115200

# WITSML Change mechanism features
#
# witsml_change_mechanism_feature=false
# witsml_change_mechanism_delay_period_in_seconds=0
#witsml_change_mechanism_detection_period_in_seconds=10
# witsml_change_mechanism_initial_last_change_feature=true
# witsml_change_mechanism_late_channels_feature=false
# witsml_change_mechanism_object_growing_feature=true
# witsml_change_mechanism_initial_last_change_in_minutes=10
```
