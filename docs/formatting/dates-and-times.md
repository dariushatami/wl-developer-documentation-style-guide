Use American English conventions for formatting all dates and times in user-facing content. Consistency ensures clarity across regions, especially for international readers who may be more familiar with day–month–year formats.

!!! note "ISO 8601 for API responses"
    
    This guidance doesn't apply to machine-readable or API responses, which must conform to ISO 8601 date-time formatting with UTC time. This includes formats like `2025-07-31T14:45:00Z` or `2025-07-31T14:45:00+00:00`. 
    
    For more details on REST and GraphQL date and time formats, see [WellnessLiving API Design Guide](https://github.com/wellnessliving-digital/api-design-guide).

## Date formatting
Use Month Day, Year (with a comma) for all full dates:
* ✅ (good) July 31, 2025
* ❌ (bad) 31 July 2025
* ❌ (bad) 2025/07/31

Avoid abbreviations like 7/31/25, which can be misread internationally.

## Time formatting
Use the 12-hour clock with lowercase a.m. / p.m., with a space between the time and the marker. Always include minutes, even for times on the hour, for consistency:
* ✅ 9:00 a.m., 3:45 p.m.
* ❌ 09:00 or 15:45
* ❌ 9am or 3PM

Use an en dash with spaces to show time ranges:
* ✅ 9:00 a.m. – 5:00 p.m.

## Time zone references
When mentioning time zones, default to Eastern Time unless otherwise specified, and include ET, EST, or EDT as appropriate:
* ✅ 2:00 p.m. ET
* ✅ 10:30 a.m. EST (winter), 10:30 a.m. EDT (summer)