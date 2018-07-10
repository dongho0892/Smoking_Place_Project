             Prefix Verb   URI Pattern                         Controller#Action
    place_registers GET    /place_registers(.:format)          place_registers#index
                    POST   /place_registers(.:format)          place_registers#create             new_place_register GET    /place_registers/new(.:format)      place_registers#new
    edit_place_register GET    /place_registers/:id/edit(.:format) place_registers#edit
         place_register GET    /place_registers/:id(.:format)      place_registers#show
                        PATCH  /place_registers/:id(.:format)      place_registers#update
                        PUT    /place_registers/:id(.:format)      place_registers#update
                        DELETE /place_registers/:id(.:format)      place_registers#destroy
                  users GET    /users(.:format)                    users#index
                        POST   /users(.:format)                    users#create
               new_user GET    /users/new(.:format)                users#new
              edit_user GET    /users/:id/edit(.:format)           users#edit
                   user GET    /users/:id(.:format)                users#show
                        PATCH  /users/:id(.:format)                users#update
                        PUT    /users/:id(.:format)                users#update
                        DELETE /users/:id(.:format)                users#destroy
          smoking_areas GET    /smoking_areas(.:format)            smoking_areas#index
                        POST   /smoking_areas(.:format)            smoking_areas#create
       new_smoking_area GET    /smoking_areas/new(.:format)        smoking_areas#new
      edit_smoking_area GET    /smoking_areas/:id/edit(.:format)   smoking_areas#edit
           smoking_area GET    /smoking_areas/:id(.:format)        smoking_areas#show
                        PATCH  /smoking_areas/:id(.:format)        smoking_areas#update
                        PUT    /smoking_areas/:id(.:format)        smoking_areas#update
                        DELETE /smoking_areas/:id(.:format)        smoking_areas#destroy
               rails_db        /rails/db                           RailsDb::Engine
               
    Routes for RailsDb::Engine:
                root GET  /                                    rails_db/dashboard#index
          table_data GET  /tables/:table_id/data(.:format)     rails_db/tables#data
           table_csv GET  /tables/:table_id/csv(.:format)      rails_db/tables#csv
      table_truncate GET  /tables/:table_id/truncate(.:format) rails_db/tables#truncate
       table_destroy GET  /tables/:table_id/destroy(.:format)  rails_db/tables#destroy
          table_edit GET  /tables/:table_id/edit(.:format)     rails_db/tables#edit
        table_update PUT  /tables/:table_id/update(.:format)   rails_db/tables#update
          table_xlsx GET  /tables/:table_id/xlsx(.:format)     rails_db/tables#xlsx
           table_new GET  /tables/:table_id/new(.:format)      rails_db/tables#new
        table_create POST /tables/:table_id/create(.:format)   rails_db/tables#create
              tables GET  /tables(.:format)                    rails_db/tables#index
               table GET  /tables/:id(.:format)                rails_db/tables#show
                 sql GET  /sql(.:format)                       rails_db/sql#index
          sql_import GET  /import(.:format)                    rails_db/sql#import
         sql_execute POST /execute(.:format)                   rails_db/sql#execute
             sql_csv POST /sql-csv(.:format)                   rails_db/sql#csv
             sql_xls POST /sql-xls(.:format)                   rails_db/sql#xls
    sql_start_import POST /import-start(.:format)              rails_db/sql#import_start
          data_table GET  /data-table(.:format)                rails_db/dashboard#data_table
          standalone GET  /standalone(.:format)                rails_db/dashboard#standalone