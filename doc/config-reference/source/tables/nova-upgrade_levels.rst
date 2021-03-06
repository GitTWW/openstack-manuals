..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _nova-upgrade_levels:

.. list-table:: Description of upgrade_levels configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description

   * - ``compute`` = ``None``

     - (String) Compute RPC API version cap.

       By default, we always send messages using the most recent version the client knows about.

       Where you have old and new compute services running, you should set this to the lowest deployed version. This is to guarantee that all services never send messages that one of the compute nodes can't understand. Note that we only support upgrading from release N to release N+1.

       Set this option to "auto" if you want to let the compute RPC module automatically determine what version to use based on the service versions in the deployment.

       Possible values:

       * By default send the latest version the client knows about

       * 'auto': Automatically determines what version to use based on the service versions in the deployment.

       * A string representing a version number in the format 'N.N'; for example, possible values might be '1.12' or '2.0'.

       * An OpenStack release name, in lower case, such as 'mitaka' or 'liberty'.

   * - ``network`` = ``None``

     - (String) Network RPC API version cap

   * - ``conductor`` = ``None``

     - (String) Conductor RPC API version cap

   * - ``cells`` = ``None``

     - (String) Cells RPC API version cap

   * - ``cert`` = ``None``

     - (String) Cert RPC API version cap

   * - ``scheduler`` = ``None``

     - (String) Scheduler RPC API version cap

   * - ``intercell`` = ``None``

     - (String) Intercell RPC API version cap

   * - ``console`` = ``None``

     - (String) Console RPC API version cap

   * - ``consoleauth`` = ``None``

     - (String) Consoleauth RPC API version cap

   * - ``baseapi`` = ``None``

     - (String) Base API RPC API version cap
