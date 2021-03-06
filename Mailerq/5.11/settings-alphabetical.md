# Configuration A-Z

This article contains a list of all configuration settings, sorted 
alphabetically. Each setting links to a documentation article that explains 
the setting more in-depth. Or do you want to [search by topic](configuration "Configure by topic")?

| Setting                                                                  | Description
|--------------------------------------------------------------------------|------------------------------------------------------------------------------------------|
| [cluster-address](cluster#config-file-options)                           | Address for a cluster to share between instances
| [cluster-exchange](cluster#config-file-options)                          | Set cluster exchange
| [cluster-timeout](cluster#command-line-option)                           | Number of seconds the --list-cluster option waits
| [cluster-verify](cluster#config-file-options)                            | Should the server certificate be verified (only used for amqps:// connections)
| [database-address](database-access#database-settings-in-the-config-file) | Relational database for config data and delivery settings
| [database-ttl](database-access#time-to-live)                             | Time to live: Database reload interval (Default 600s)
| [database-validate](database-access#fixing-values-in-the-database)       | Check and fix database settings on startup
| [download-blacklist](responsiveemail#firewall-bypass)                    | IP addresses from which no resources can be downloaded
| [download-cache](responsiveemail#config-file-variables)                  | Address of the cache (Used in ResponsiveEmail)
| [download-log-format](logging#download-logs)                             | Download log format
| [download-log-file](logging#download-logs)                               | Download log filename
| [download-ttl](responsiveemail#config-file-variables)                    | Max time to keep downloaded resources in the cache (Used in ResponsiveEmail)
| [download-whitelist](responsiveemail#firewall-bypass)                    | Exceptions to the download-blacklist
| [download-proxy](responsiveemail)                                        | Route outgoing download requests through a proxy
| [dsn-advertise](sending-bounces#receiving-dsn-settings)                  | Toggle announcement about DSN extension and parameters
| [dsn-notify](sending-bounces#mime-headers-and-config-file-settings)      | Events that trigger a notify
| [dsn-ret](sending-bounces#passing-dsn-settings)                          | Send full mail (FULL) or headers (HDRS) for notifications
| [dns-min-ttl](dns-settings)                                              | Minimum TTL to respect when doing domain lookups
| [error-log](logging#error-logs)                                          | Full path to the error log
| [heartbeat-enabled](other-configuration#user-statistics)                 | Toggle user statistics (default: true)
| [license](other-configuration#license)                                   | MailerQ license file
| [lock](other-configuration#lockfile)                                     | Process ID for MailerQ instance to prevent from starting instances more than once
| [max-attempts](other-configuration)                                      | Maximum attempts to deliver email
| [max-delivertime](other-configuration)                                   | Maximum time spent trying to deliver email
| [plugin-directory](plugins#how-are-plugins-loaded)                       | Directory with MailerQ plugins
| [proxy-server](other-configuration)                                      | Setup proxy for outgoing HTTP requests
| [rabbitmq-address](rabbitmq-config#rabbitmq-address)                     | Location and authentication to connect to RabbitMQ
| [rabbitmq-consumers](rabbitmq-config#multiple-threads)                   | Amount of consumer threads (default: 1)
| [rabbitmq-declare](rabbitmq-config#disable-startup-declarations)         | Enable or disable checking and declaring the queues on startup  
| [rabbitmq-dsn](rabbitmq-config#rabbitmq-queues)                          | Your RabbitMQ delivery status notification queue  
| [rabbitmq-durable](rabbitmq-config#persistent-and-durable-settings)      | Durable/not durable RabbitMQ queues (default: true)
| [rabbitmq-encoding](rabbitmq-config#compression)                         | Choose encoding for messages (such as gzip)
| [rabbitmq-exchange](rabbitmq-config#the-exchange)                        | RabbitMQ exchange
| [rabbitmq-failure](rabbitmq-config#rabbitmq-queues)                      | Your RabbitMQ failure queue
| [rabbitmq-inbox](rabbitmq-config#rabbitmq-queues)                        | Your RabbitMQ inbox queue
| [rabbitmq-local](rabbitmq-config#rabbitmq-queues)                        | Your RabbitMQ local queue 
| [rabbitmq-lazy](rabbitmq-config#persisten-and-durable-settings)          | Lazy/non lazy RabbitMQ queues (default: non-lazy)
| [rabbitmq-maxpriority](rabbitmq-config#priority-queues)                  | Enable the use of priority queues 
| [rabbitmq-qos](rabbitmq-config#quality-of-service)                       | Set a maximum number of messages simultaneously consumed per consumer thread
| [rabbitmq-minqos](rabbitmq-config#quality-of-service)                    | Set a minimum number of messages simultaneously consumed per consumer thread
| [rabbitmq-flush-qos](rabbitmq-config#quality-of-service)                 | Set a maximum number of messages simultaneously consumed during flush
| [rabbitmq-outbox](rabbitmq-config#rabbitmq-queues)                       | Your RabbitMQ outbox queue (must be unique if multiple instances of MailerQ are used)
| [rabbitmq-persistent](rabbitmq-config#persistent-and-durable-settings)   | Persistent/not persistent RabbitMQ queues (default: false)
| [rabbitmq-publishers](rabbitmq-config#multiple-threads)                  | Amount of publisher threads (default: 1)
| [rabbitmq-queues](rabbitmq-config#rabbitmq-queues)                       | Names of the RabbitMQ queues to manage email (inbox, failures, retries, etc...)
| [rabbitmq-refused](rabbitmq-config#rabbitmq-queues)                      | Your RabbitMQ refused queue
| [rabbitmq-reports](rabbitmq-config#rabbitmq-queues)                      | Your RabbitMQ report queue
| [rabbitmq-results](rabbitmq-config#rabbitmq-queues)                      | Your RabbitMQ result queue
| [rabbitmq-retry](rabbitmq-config#rabbitmq-queues)                        | Your RabbitMQ retry queue
| [rabbitmq-success](rabbitmq-config#rabbitmq-queues)                      | Your RabbitMQ success queue
| [rabbitmq-verify](rabbitmq-config#rabbitmq-address)                      | Should the server certificate be verified (only used for amqps:// connections)
| [received-log-format](logging#received-messages)                         | Received log format
| [received-log-file](logging#received-messages)                           | Received log filename
| [retry-interval](other-configuration)                                    | Interval for retrying to send
| [send-bin-log-file](logging#send-logs)                                   | Binary send log filename
| [send-log-file](logging#send-logs)                                       | Send log filename
| [send-log-format](logging#send-logs)                                     | Send log format
| [server-id](multiple-instances#server-id)                                | Server ID to prevent multiple instances from assigning same message ID
| [smarthost](smarthost#how-to-configure-the-smarthost-feature)            | Smarthost name (only needed if Smarthost is desired)
| [smarthost-password](smarthost#how-to-configure-the-smarthost-feature)   | Smarthost password
| [smarthost-port](smarthost#how-to-configure-the-smarthost-feature)       | Smarthost port
| [smarthost-username](smarthost#how-to-configure-the-smarthost-feature)   | Smarthost username
| [smtp-auth-results](smtp-server#testing-incoming-messages)               | Toggle adding authentication results to MIME header
| [smtp-certificate](smtp-server#secure-connections)                       | Certificate for secure SMTP connections
| [smtp-check](smtp-server#testing-incoming-messages)                      | Comma separated list of checks to perform on incoming messages
| [smtp-ciphers](smtp-server#secure-connections)                           | Supported ciphers for secure SMTP connections
| [smtp-connections](smtp-server#other-settings)                           | Maximum amount of open TCP connections allowed
| [smtp-default-ips](smtp-server#config-file-settings)                     | List of default outgoing IP addresses
| [smtp-extract](smtp-server#mime-headers)                                 | Toggle automatic extraction of metadata
| [smtp-ip](smtp-server#config-file-settings)                              | SMTP server IP
| [smtp-key](smtp-server#secure-connections)                               | Private key for secure SMTP connections
| [smtp-mappable-ips](smtp-server#config-file-settings)                    | List of mappable IP adresses
| [smtp-maxsize](smtp-server#other-settings)                               | Maximum message size to accept
| [smtp-password](smtp-server#controlling-access)                          | Password for authenticating to SMTP server
| [smtp-port](smtp-server#config-file-settings)                            | Ports for incoming MailerQ connections
| [smtp-proxy](smtp-server#running-behind-haproxy)                         | IPs to treat as connection from proxy server
| [smtp-range](smtp-server#controlling-access)                             | Range of IP address to allow incoming email for
| [smtp-secure port](smtp-server#config-file-settings)                     | Ports for secure incoming MailerQ connections
| [smtp-sink-address](smarthost#using-smarthost-for-debugging)             | SMTP sink domain name or ip address
| [smtp-sink-password](smarthost#using-smarthost-for-debugging)            | SMTP sink password
| [smtp-sink-port](smarthost#using-smarthost-for-debugging)                | SMTP sink port
| [smtp-sink-username](smarthost#using-smarthost-for-debugging)            | SMTP sink username
| [smtp-threads](smtp-server#other-settings)                               | Number of threads started for SMTP traffic
| [smtp-timeout](smtp-server#other-settings)                               | Max idle time on incoming SMTP connections
| [smtp-protection](smtp-server#other-settings)                            | Enable SMTP incoming IP blacklist
| [smtp-unmappable-ips](smtp-server#config-file-settings)                  | List of unmappable IP addresses
| [smtp-username](smtp-server#controlling-access)                          | Username for authenticating to SMTP server
| [spamassassin-host](smtp-server#testing-incoming-messages)               | Address for SpamAssassin daemon 
| [spamassassin-port](smtp-server#testing-incoming-messages)               | Port for SpamAssassin daemon
| [spool-delay](spool-directory#config-file-options)                       | Delay for processing spool directory files
| [spool-directory](spool-directory#config-file-options)                   | Path to the directory to monitor
| [spool-extract](spool-directory#config-file-options)                     | Toggle scanning for headers in spool directory mail
| [spool-fail-directory](spool-directory#config-file-options)              | Path to move files to that could not be picked up
| [spool-open-files](spool-directory#config-file-options)                  | Amount of files that may be open simultaneously by the spool directory                    
| [spool-remove](spool-directory#config-file-options)                      | Toggle removal of files from spool directory
| [spool-threads](spool-directory#config-file-options)                     | Amount of threads to use for the spool directory
| [storage-address](message-store-options)                                 | Address for external message storage
| [storage-policy](message-store-options)                                  | Message store policy
| [storage-reschedule](message-store-options)                              | Number of seconds to wait before a mail is retried
| [storage-threads](message-store-options)                                 | Storage threads
| [storage-timeout](message-store-options)                                 | Timeout for fetch operations
| [storage-ttl](message-store-options)                                     | Time to live: Storage reload interval
| [user](other-configuration#user)                                         | Change user for MTA
| [validate-envelope](other-configuration)                                 | Validate envelope address before sending
| [validate-recipient](other-configuration)                                | Validate recipient address before sending
| [www-cache-control](mgmt-setup#advanced-caching-options)                 | Enable or disable browser cache
| [www-certificate](mgmt-setup#setting-up-a-secure-management-console)     | Certificate file for secure connection to management console
| [www-ciphers](mgmt-setup#setting-up-a-secure-management-console)         | Supported ciphers for secure management console
| [www-connections](mgmt-setup#activation)                                 | Limit for simultaneous HTTP connections to built-in HTTP server
| [www-ip](multiple-instances#listening-ip/ports-combinations)             | Web interface IP (IP/port combination unique for every instance of MailerQ)
| [www-dir](mgmt-setup#activation)                                         | Directory for installing MailerQ management console files
| [www-host](multiple-instances#listening-ip/ports-combinations)           | Web interface host (IP/port combination unique for every instance of MailerQ)
| [www-password](mgmt-setup#activation)                                    | Management console password
| [www-port](mgmt-setup#activation)                                        | Port number for the management console
| [www-private-key](mgmt-setup#setting-up-a-secure-management-console)     | Private key for secure connection to management console
| [www-secure-port](mgmt-setup#setting-up-a-secure-management-console)     | Secure (HTTPS) port number for the management console
| [www-url](mgmt-setup#announcing-the-interface-on-the-cluster)            | The URL via which the management console is accessible

## Boolean options

To check your version of MailerQ for example, just type in the cli:

```txt
$ mailerq --version
```

| Setting                     | Description
|-----------------------------|--------------------------------------------------------|
| daemon                      | Deamon process (deafault true)
| disable-crash-report        | Disable crash report
| disable-crash-post          | Disable automatic crash posting
| extract-recipients          | Read in a mime message from standard input and filter out the destination addresses
| ignore-dot                  | Instruct MailerQ that dots do not have a special meaning
| list-ips                    | List IP addresses
| loopback                    | Loopback
| notify-cluster              | Notify cluster
| paused                      | Pause
| purge-database              | Rebuilding the database tables
| repair-database             | Repair the database
| version                     | Version

