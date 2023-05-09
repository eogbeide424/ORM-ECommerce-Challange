


# ORM E-Commerce-Challange
|Javascript  | https://github.com/eogbeide424/ORM-ECommerce-Challange| 
|Walk through link | https://drive.google.com/file/d/120nWKo8Zhakzs8eZdwfXXo8zHfBOpUxC/view?usp=sharing | 

## Description

 On this project our task was to connect mysql to an enviroment variable file, then when entering the schema and seeds commands to have the database deployed also we had to implement all the routes for the models that was built so when you use insomia the post routes and get routes to all  the models work and also the put routes



 ## Code Snippetts
 this snippet was what I used to find the and isolate a single category by finding it by the primary key I found that using sequelize actually makes working with mysql easier to read and work with 

  ```
     try{
    const categoryData= await Category.findByPk(req.params.id, {
      include: [{model: Product}]
    });

    if(!categoryData){
      res.status(404).json({message: 'No category found with that id'});
      return;
    }
    res.status(200).json(categoryData);
  } catch (err){
    res.status(500).json(err);
  }
  ```

## Table of Contents (Optional)

If your README is very long, add a table of contents to make it easy for users to find what they need.

* [Installation](#installation)
* [Usage](#usage)
* [Credits](#credits)
* [License](#license)


## Installation

to install the please run npm install before using 


## Usage 

to use please enter the schema to create the database then seed the database. After that please start by doing an npm start 



## Credits

Eugene Ogbeide eogbeide2@gmail.com

## License

MIT

'https://choosealicense.com/licenses/MIT/

undefined



---

🏆 The sections listed above are the minimum for a good README, but your project will ultimately determine the content of this document. You might also want to consider adding the following sections.

## Badges


https://img.shields.io/badge/license-MIT-red

## Questions
If any questions on how to use the app you can email me at eogbeide2@gmail.com

© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
