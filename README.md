This program converts a log file to csv for better viewing.
A snippet of the log file:
2017-11-23 06:00:03,400 [6631:son.infra.kqi_collector.cellmining.base:23:inner:INFO] Event=Start Method=__init__ a=(<son.infra.kqi_collector.cellmining.roads.CellMiningCellsOnRoadReader object at 0x2b5b307cfd10>,) kw={'cgi_map': <son.infra.store.cell_kqi.CGICellIDMap object at 0x2b5b2fea8f10>, 'rats': ['UMTS', 'LTE'], 'market': 'M4', 'database': u'ETL'}
2017-11-23 06:00:03,400 [6631:son.infra.kqi_collector.cellmining.base:25:inner:INFO] Event=Done Method=__init__ rv=None
2017-11-23 06:00:03,400 [6631:son.infra.kqi_collector.cellmining.base:23:inner:INFO] Event=Start Method=construct_query a=(<son.infra.kqi_collector.cellmining.roads.CellMiningCellsOnRoadReader object at 0x2b5b307cfd10>,) kw={}
2017-11-23 06:00:03,401 [6631:son.infra.kqi_collector.cellmining.base:25:inner:INFO] Event=Done Method=construct_query rv={'query': "ETL.dbo.usp_CellsPerRoad_Filter @Road_ID='0',@RAT='UMTS,LTE'"}
2017-11-23 06:00:03,418 [6631:son.infra.kqi_collector.cellmining.sql:60:connect:INFO] Event=CONNECTED user=sondev_2 CellMiningSQLServer=ic-phy-217-cm.cisco.com:2382
2017-11-23 06:00:03,999 [6631:son.infra.kqi_collector.cellmining.base:23:inner:INFO] Event=Start Method=process_response a=(<son.infra.kqi_collector.cellmining.roads.CellMiningCellsOnRoadReader object at 0x2b5b307cfd10>, <pymssql.Cursor object at 0x2b5b30790460>) kw={}
2017-11-23 06:00:25,770 [6631:son.infra.kqi_collector.cellmining.roads:82:update_road:INFO] {'market': u'M4', 'proc': 'CellMiningCellsOnRoadReader', 'event': 'NO_CHANGE_IN_CELLS', 'road': 1104}
2017-11-23 06:00:25,773 [6631:son.infra.kqi_collector.cellmining.roads:82:update_road:INFO] {'market': u'M4', 'proc': 'CellMiningCellsOnRoadReader', 'event': 'NO_CHANGE_IN_CELLS', 'road': 588}
2017-11-23 06:00:25,775 [6631:son.infra.kqi_collector.cellmining.roads:82:update_road:INFO] {'market': u'M4', 'proc': 'CellMiningCellsOnRoadReader', 'event': 'NO_CHANGE_IN_CELLS', 'road': 528}
