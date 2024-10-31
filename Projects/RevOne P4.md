#### How to spin up frontend
Start codespace then spin up locally using

	bcompile
	bdeploy
	fdeploy

package.json has scripts to start up dev,stage,etc

have to go into ec2/ecr to deploy change after pull request
####  is all the data located for the deduplication
account number is in

	galaxy.utxn_perfiniti_medicare

data mapping is in

	SELECT *
	FROM galaxy.mst_dm_record_field_map
	where record_code = 'Perfiniti SF OPP DUP'

#### Other
	LOGGER.info(msg: String);
alternatively

	LOGGER.info(String.format("log msg", CommonUtils.getString(null)))

