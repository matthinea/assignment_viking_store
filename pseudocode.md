


User
  email - string - required
  name - string - required
  phone number - string
  default\_billing\_address\_foreign_key
  default\_shipping\_address\_foreign_key

Order
  phone number - string - required
  placed - boolean - default:false
  delivered - boolean - default:false
  user\_foreign\_key - integer - required
  shipping\_address\_foreign_key - integer - required 
  billing\_address\_foreign_key - integer - required

Product/Order 
  product_id - integer
  order_id - integer
  no\_of\_items - integer

Product
  title - string
  description - text
  price - float
  sku - string
  category\_foreign\_key - integer

Category
  title - string
  description - text

Address
  street_address - string
  city - string
  state - string
  zip - string
  country - string 
  default - boolean default:false
  billing\_or\_shipping - binary - default:shipping
  user\_foreign\_key - integer

Credit Card
  vendor - string - required
  number - integer - required
  csc - integer - required
  expiration - date - required
  user\_foreign\_key - integer
