# onepassword_item_document

This resource can load any document from 1password.

## Example Usage

```hcl
data "onepassword_item_document" "this" {
    name = "some-document-from-vault"
}
```

## Argument Reference

* `name` - (Required) your document title.
* `field_path` - (Required) path to your document, which will be upload to 1password.
* `vault` - (Optional) see details in onepassword_item_common.
* `notes` - (Optional) see details in onepassword_item_common.
* `tags` - (Optional) see details in onepassword_item_common.
* `section` - (Optional) see details in onepassword_item_common.

## Attribute Reference

In addition to the above arguments, the following attributes are exported:

* `id` - document id.
* `content` - document content.
