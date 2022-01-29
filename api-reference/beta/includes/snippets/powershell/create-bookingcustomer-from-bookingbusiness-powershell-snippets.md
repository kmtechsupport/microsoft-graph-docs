---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
	DisplayName = "Joni Sherman"
	EmailAddress = "jonis@relecloud.com"
	Addresses = @(
		@{
			PostOfficeBox = ""
			Street = "4567 Main Street"
			City = "Buffalo"
			State = "NY"
			CountryOrRegion = "USA"
			PostalCode = "98052"
			Type = "home"
		}
		@{
			PostOfficeBox = ""
			Street = "4570 Main Street"
			City = "Buffalo"
			State = "NY"
			CountryOrRegion = "USA"
			PostalCode = "98054"
			Type = "business"
		}
	)
	Phones = @(
		@{
			Number = "206-555-0100"
			Type = "home"
		}
		@{
			Number = "206-555-0200"
			Type = "business"
		}
	)
}

New-MgBookingBusinessCustomer -BookingBusinessId $bookingBusinessId -BodyParameter $params

```