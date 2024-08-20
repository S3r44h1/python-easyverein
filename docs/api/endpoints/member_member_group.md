| API Endpoint                | Namespace                                          | Supported Generics |
|-----------------------------|----------------------------------------------------|--------------------|
| `member/<member_id>/groups` | `evclient.member.member_groups(<member>).<method>` | CRUD               |

## Additional parameters

As member related custom fields are always bound to a specific member, the namespace used for custom field associations
requires the member as constructor argument, to avoid passing it again to all endpoints:

| Name     | Type    | Description | Default                                                                                           |
|----------|---------|-------------|---------------------------------------------------------------------------------------------------|
| `member` | `Member | int`        | Identifies the member to modify custom field values on. Can be either an id or a `Member` object. | *required* |

## Generic Model Mappings

| Generic Model     | Invoice Model             |
|-------------------|---------------------------|
| `ModelType`       | `MemberMemberGroup`       |
| `CreateModelType` | `MemberMemberGroupCreate` |
| `UpdateModelType` | `MemberMemberGroupUpdate` |

## Additional Methods

::: easyverein.modules.member_member_group.MemberMemberGroupMixin
    options:
        inherited_members: false
        show_signature: true
        show_signature_annotations: true
        show_root_heading: false
        show_bases: false
        show_root_toc_entry: false
        separate_signature: true
        heading_level: 3
        filters:
            - "!^c$"
            - "!^logger$"
            - "!^endpoint_name"
            - "!^return_type"