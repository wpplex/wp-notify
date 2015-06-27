# wp-notify
A small notification class to manage your WordPress Admin Notifications.

## Usage

First, you init your class with a custom prefix (namespace for your notifications)

```
$notify = new wpplex\WP_Notify\WP_Notify( 'my-notif' );
```

Create your first notification

```
$id = 'notif-xxy';
$content = 'some random notif text';
$type = 'error';
$hide_button = true;
$notify->add_notification( $id, $content, $type, $hide_button );
```

Display your notification

```
$id = 'notif-xxy';
$display_count = 20; // times
$notify->display_notification( $id, $display_count );
```

Hide your notification

```
$id = 'notif-xxy';
$notify->hide_notification( $id );
```
