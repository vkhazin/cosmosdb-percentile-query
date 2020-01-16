# Cosmos DB Percentile Query

## Objectives

* Use Cosmos db with Core Sql API 
* Write query to calculate difference in msec between two date-time fields: `SourceTimestamp` and `SyncTimestamp`
* The query is to calculate 95% percentile of the difference between `SourceTimestamp` and `SyncTimestamp`, e.g. for the 95% of records in the table, the difference is no more than 5,178 msec

## Sample Cosmos DB Data 

```
{
	"FareTypeId": 1,
	"FareTypeAbbr": "STA",
	"Description": "Standard Fare",
	"FlatRate": 2.0,
	"DistanceRate": 0.0,
	"PolygonRate": 0.0,
	"TimeRate": 0.0,
	"PolyTypeId": 0,
	"FareAdjustDiffZon": 0.0,
	"FareAdjustSameZon": 0.0,
	"DistanceLimitSameZon": 0.0,
	"DistanceLimitDiffZon": 0.0,
	"NumCode": 1,
	"FareMode": 0,
	"FareCalcType": 0,
	"SourceTimestamp": "2002-10-02T15:00:00.05456Z",
	"SyncTimestamp": "2002-10-02T15:00:01.05789Z"
}
```

## Deliverables

* Sample dataset no less than 100 records
* Query and user-defined functions if required
* README.MD using markdown documentation on how to setup and to run
* A walk through using shared screen testing on a new environment 