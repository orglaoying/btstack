
# Makefile to build and run all tests

SUBDIRS =  \
	att_db_util \
	ble_client \
	des_iterator \
	gatt_client \
	linked_list \
	remote_device_db \
	sdp_client \
	security_manager \

EXCLUDED = ios

subdirs:
	echo Building all tests
	for dir in $(SUBDIRS); do \
	  $(MAKE) -C $$dir; \
	done

clean:
	echo Clean all test
	for dir in $(SUBDIRS); do \
	  $(MAKE) -C $$dir clean; \
	done

test:
	echo Run all test
	for dir in $(SUBDIRS); do \
	  $(MAKE) -C $$dir test; \
	done


