bin_PROGRAMS = sciphi convertTree2Map createSingleCellTree sciphi_test

sciphi_SOURCES = \
	src/findBestTrees.cpp

sciphi_CXXFLAGS = \
	$(PTHREAD_CFLAGS) $(GSL_CFLAGS)

sciphi_CPPFLAGS = \
	$(DLIB_CPPFLAGS) -I$(DLIB_INCLUDEDIR) $(BOOST_CPPFLAGS) @BOOST_UNIT_TEST_FRAMEWORK_CPPFLAGS@

sciphi_LDADD = \
	$(GSL_LIBS) $(BOOST_LDFLAGS) $(BOOST_SYSTEM_LIB) $(BOOST_PROGRAM_OPTIONS_LIB) $(BOOST_FILESYSTEM_LIB) $(BOOST_IOSTREAMS_LIB) $(DLIB_LDFLAGS)

convertTree2Map_SOURCES = \
	src/convertTreeIntoClusterMap.cpp

convertTree2Map_CXXFLAGS = \
	$(PTHREAD_CFLAGS) $(GSL_CFLAGS)

convertTree2Map_CPPFLAGS = \
	$(BOOST_CPPFLAGS) @BOOST_UNIT_TEST_FRAMEWORK_CPPFLAGS@

convertTree2Map_LDADD = \
	$(GSL_LIBS) $(BOOST_LDFLAGS) $(BOOST_SYSTEM_LIB) $(BOOST_PROGRAM_OPTIONS_LIB) $(BOOST_FILESYSTEM_LIB) $(BOOST_IOSTREAMS_LIB) -lboost_graph -lboost_regex

createSingleCellTree_SOURCES = \
	src/createSingleCellSeqTree.cpp

createSingleCellTree_CXXFLAGS = \
	$(PTHREAD_CFLAGS)

createSingleCellTree_CPPFLAGS = \
	-I$(SEQAN_INCLUDEDIR) $(BOOST_CPPFLAGS) $(ZLIB_CFLAGS) @BOOST_UNIT_TEST_FRAMEWORK_CPPFLAGS@

createSingleCellTree_LDADD = \
	$(ZLIB_LIBS) $(BOOST_LDFLAGS) $(BOOST_UNIT_TEST_FRAMEWORK_LIB) $(PTHREAD_CFLAGS)

sciphi_test_SOURCES = \
	test/sciphi_test.cpp

sciphi_test_CXXFLAGS = \
	$(PTHREAD_CFLAGS) $(GSL_CFLAGS)

sciphi_test_CPPFLAGS = \
	$(DLIB_CPPFLAGS) -I$(DLIB_INCLUDEDIR) $(BOOST_CPPFLAGS) @BOOST_UNIT_TEST_FRAMEWORK_CPPFLAGS@

sciphi_test_LDADD = \
	$(GSL_LIBS) $(BOOST_LDFLAGS) $(BOOST_SYSTEM_LIB) $(BOOST_PROGRAM_OPTIONS_LIB) $(BOOST_FILESYSTEM_LIB) $(BOOST_IOSTREAMS_LIB) $(DLIB_LDFLAGS) $(BOOST_UNIT_TEST_FRAMEWORK_LIB)
