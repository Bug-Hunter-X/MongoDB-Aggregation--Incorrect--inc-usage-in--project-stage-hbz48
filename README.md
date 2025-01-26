# MongoDB Aggregation Pipeline Error: Incorrect $inc Usage
This repository demonstrates a common error encountered when using the `$inc` operator within the `$project` stage of a MongoDB aggregation pipeline. The `$inc` operator is designed to increment a numeric field, but using it incorrectly with an array leads to an error. The solution shows the correct way to implement the incrementation.

## Bug
The bug lies in the `$project` stage of the aggregation pipeline.  The `$inc` operator is incorrectly applied to an array, causing the pipeline to fail. 

## Solution
The solution demonstrates the correct usage of `$inc` in the `$project` stage by applying it directly to the `count` field.