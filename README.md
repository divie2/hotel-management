# Hotel Management API

This API provides endpoints to manage room types and rooms in a hotel.

## Endpoints

### GET {localhost}/api/v1/room-types

Fetch all room types.

#### Example:
curl http://localhost:3000/api/v1/room-types


### POST /api/v1/room-types

Create a new room type.

#### Example:
curl -X POST -H "Content-Type: application/json" -d '{"name": "Suite 3"}' http://localhost:3000/api/v1/room-types



### GET /api/v1/rooms

Fetch all rooms.

#### Example:
curl http://localhost:3000/api/v1/rooms



### POST /api/v1/rooms

Create a new room.

#### Example:
curl -X POST -H "Content-Type: application/json" -d '{"name": "Room 101", "roomType": "roomTypeId", "price": 100}' http://localhost:3000/api/v1/rooms


Replace `"roomTypeId"` with the actual ID of the room type.

### PATCH /api/v1/rooms/{roomId}

Update a specific room by ID.

#### Example:
curl -X PATCH -H "Content-Type: application/json" -d '{"price": 120}' http://localhost:3000/api/v1/rooms/roomId



Replace `"roomId"` with the actual ID of the room.

### DELETE /api/v1/rooms/{roomId}

Delete a specific room by ID.

#### Example:
curl -X DELETE http://localhost:3000/api/v1/rooms/roomId


Replace `"roomId"` with the actual ID of the room.

### GET /api/v1/rooms/{roomId}

Fetch a specific room by ID.

#### Example:
curl http://localhost:3000/api/v1/rooms/roomId
Replace `"roomId"` with the actual ID of the room.

You can also physically visuallize this rooms using PC mongodb application



