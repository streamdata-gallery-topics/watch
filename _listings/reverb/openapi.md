---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cart/move_to_watch_list/{cart_item_id}:
    post:
      summary: Post Cart Move To Watch List Cart Item
      description: Remove a cart item and add it to watch list
      operationId: postCartMoveToWatchListCartItem
      x-api-path-slug: cartmove-to-watch-listcart-item-id-post
      parameters:
      - in: path
        name: cart_item_id
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Move
      - To
      - Watch
      - List
      - Cart
      - Item
      - Id
---