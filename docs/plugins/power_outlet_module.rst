.. Document meta

:orphan:

.. Anchors

.. _ansible_collections.networktocode.nautobot.power_outlet_module:

.. Anchors: short name for ansible.builtin

.. Anchors: aliases



.. Title

networktocode.nautobot.power_outlet -- Create, update or delete power outlets within Nautobot
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

.. Collection note

.. note::
    This plugin is part of the `networktocode.nautobot collection <https://galaxy.ansible.com/networktocode/nautobot>`_ (version 3.1.1).

    To install it use: :code:`ansible-galaxy collection install networktocode.nautobot`.

    To use it in a playbook, specify: :code:`networktocode.nautobot.power_outlet`.

.. version_added

.. versionadded:: 1.0.0 of networktocode.nautobot

.. contents::
   :local:
   :depth: 1

.. Deprecated


Synopsis
--------

.. Description

- Creates, updates or removes power outlets from Nautobot


.. Aliases


.. Requirements

Requirements
------------
The below requirements are needed on the host that executes this module.

- pynautobot


.. Options

Parameters
----------

.. raw:: html

    <table  border=0 cellpadding=0 class="documentation-table">
        <tr>
            <th colspan="1">Parameter</th>
            <th>Choices/<font color="blue">Defaults</font></th>
                        <th width="100%">Comments</th>
        </tr>
                    <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-description"></div>
                    <b>description</b>
                    <a class="ansibleOptionLink" href="#parameter-description" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Description of the power outlet</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-device"></div>
                    <b>device</b>
                    <a class="ansibleOptionLink" href="#parameter-device" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">raw</span>
                                                 / <span style="color: red">required</span>                    </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>The device the power outlet is attached to</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-feed_leg"></div>
                    <b>feed_leg</b>
                    <a class="ansibleOptionLink" href="#parameter-feed_leg" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li>A</li>
                                                                                                                                                                                                <li>B</li>
                                                                                                                                                                                                <li>C</li>
                                                                                    </ul>
                                                                            </td>
                                                                <td>
                                            <div>The phase, in case of three-phase feed</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-name"></div>
                    <b>name</b>
                    <a class="ansibleOptionLink" href="#parameter-name" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                 / <span style="color: red">required</span>                    </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>The name of the power outlet</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-power_port"></div>
                    <b>power_port</b>
                    <a class="ansibleOptionLink" href="#parameter-power_port" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">raw</span>
                                                                    </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>The attached power port</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-query_params"></div>
                    <b>query_params</b>
                    <a class="ansibleOptionLink" href="#parameter-query_params" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=string</span>                                            </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>This can be used to override the specified values in ALLOWED_QUERY_PARAMS that is defined</div>
                                            <div>in plugins/module_utils/utils.py and provides control to users on what may make</div>
                                            <div>an object unique in their environment.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-state"></div>
                    <b>state</b>
                    <a class="ansibleOptionLink" href="#parameter-state" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li>absent</li>
                                                                                                                                                                                                <li><div style="color: blue"><b>present</b>&nbsp;&larr;</div></li>
                                                                                    </ul>
                                                                            </td>
                                                                <td>
                                            <div>Use <code>present</code> or <code>absent</code> for adding or removing.</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-tags"></div>
                    <b>tags</b>
                    <a class="ansibleOptionLink" href="#parameter-tags" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">list</span>
                         / <span style="color: purple">elements=raw</span>                                            </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>Any tags that the power outlet may need to be associated with</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-token"></div>
                    <b>token</b>
                    <a class="ansibleOptionLink" href="#parameter-token" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                 / <span style="color: red">required</span>                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>The token created within Nautobot to authorize API access</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-type"></div>
                    <b>type</b>
                    <a class="ansibleOptionLink" href="#parameter-type" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                                    </div>
                                          <div style="font-style: italic; font-size: small; color: darkgreen">
                        added in 3.0.0 of networktocode.nautobot
                      </div>
                                                        </td>
                                <td>
                                                                                                                            <ul style="margin: 0; padding: 0"><b>Choices:</b>
                                                                                                                                                                <li>iec-60320-c5</li>
                                                                                                                                                                                                <li>iec-60320-c7</li>
                                                                                                                                                                                                <li>iec-60320-c13</li>
                                                                                                                                                                                                <li>iec-60320-c15</li>
                                                                                                                                                                                                <li>iec-60320-c19</li>
                                                                                                                                                                                                <li>iec-60309-p-n-e-4h</li>
                                                                                                                                                                                                <li>iec-60309-p-n-e-6h</li>
                                                                                                                                                                                                <li>iec-60309-p-n-e-9h</li>
                                                                                                                                                                                                <li>iec-60309-2p-e-4h</li>
                                                                                                                                                                                                <li>iec-60309-2p-e-6h</li>
                                                                                                                                                                                                <li>iec-60309-2p-e-9h</li>
                                                                                                                                                                                                <li>iec-60309-3p-e-4h</li>
                                                                                                                                                                                                <li>iec-60309-3p-e-6h</li>
                                                                                                                                                                                                <li>iec-60309-3p-e-9h</li>
                                                                                                                                                                                                <li>iec-60309-3p-n-e-4h</li>
                                                                                                                                                                                                <li>iec-60309-3p-n-e-6h</li>
                                                                                                                                                                                                <li>iec-60309-3p-n-e-9h</li>
                                                                                                                                                                                                <li>nema-5-15r</li>
                                                                                                                                                                                                <li>nema-5-20r</li>
                                                                                                                                                                                                <li>nema-5-30r</li>
                                                                                                                                                                                                <li>nema-5-50r</li>
                                                                                                                                                                                                <li>nema-6-15r</li>
                                                                                                                                                                                                <li>nema-6-20r</li>
                                                                                                                                                                                                <li>nema-6-30r</li>
                                                                                                                                                                                                <li>nema-6-50r</li>
                                                                                                                                                                                                <li>nema-l5-15r</li>
                                                                                                                                                                                                <li>nema-l5-20r</li>
                                                                                                                                                                                                <li>nema-l5-30r</li>
                                                                                                                                                                                                <li>nema-l5-50r</li>
                                                                                                                                                                                                <li>nema-l6-20r</li>
                                                                                                                                                                                                <li>nema-l6-30r</li>
                                                                                                                                                                                                <li>nema-l6-50r</li>
                                                                                                                                                                                                <li>nema-l14-20r</li>
                                                                                                                                                                                                <li>nema-l14-30r</li>
                                                                                                                                                                                                <li>nema-l21-20r</li>
                                                                                                                                                                                                <li>nema-l21-30r</li>
                                                                                                                                                                                                <li>CS6360C</li>
                                                                                                                                                                                                <li>CS6364C</li>
                                                                                                                                                                                                <li>CS8164C</li>
                                                                                                                                                                                                <li>CS8264C</li>
                                                                                                                                                                                                <li>CS8364C</li>
                                                                                                                                                                                                <li>CS8464C</li>
                                                                                                                                                                                                <li>ita-e</li>
                                                                                                                                                                                                <li>ita-f</li>
                                                                                                                                                                                                <li>ita-g</li>
                                                                                                                                                                                                <li>ita-h</li>
                                                                                                                                                                                                <li>ita-i</li>
                                                                                                                                                                                                <li>ita-j</li>
                                                                                                                                                                                                <li>ita-k</li>
                                                                                                                                                                                                <li>ita-l</li>
                                                                                                                                                                                                <li>ita-m</li>
                                                                                                                                                                                                <li>ita-n</li>
                                                                                                                                                                                                <li>ita-o</li>
                                                                                                                                                                                                <li>hdot-cx</li>
                                                                                    </ul>
                                                                            </td>
                                                                <td>
                                            <div>The type of the power outlet</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-url"></div>
                    <b>url</b>
                    <a class="ansibleOptionLink" href="#parameter-url" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">string</span>
                                                 / <span style="color: red">required</span>                    </div>
                                                        </td>
                                <td>
                                                                                                                                                            </td>
                                                                <td>
                                            <div>URL of the Nautobot instance resolvable by Ansible control host</div>
                                                        </td>
            </tr>
                                <tr>
                                                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="parameter-validate_certs"></div>
                    <b>validate_certs</b>
                    <a class="ansibleOptionLink" href="#parameter-validate_certs" title="Permalink to this option"></a>
                    <div style="font-size: small">
                        <span style="color: purple">raw</span>
                                                                    </div>
                                                        </td>
                                <td>
                                                                                                                                                                                                                <b>Default:</b><br/><div style="color: blue">"yes"</div>
                                    </td>
                                                                <td>
                                            <div>If <code>no</code>, SSL certificates will not be validated. This should only be used on personally controlled sites using self-signed certificates.</div>
                                                        </td>
            </tr>
                        </table>
    <br/>

.. Notes

Notes
-----

.. note::
   - Tags should be defined as a YAML list
   - This should be ran with connection ``local`` and hosts ``localhost``

.. Seealso


.. Examples

Examples
--------

.. code-block:: yaml+jinja

    
    - name: "Test Nautobot modules"
      connection: local
      hosts: localhost
      gather_facts: False

      tasks:
        - name: Create power port within Nautobot with only required information
          networktocode.nautobot.power_outlet:
            url: http://nautobot.local
            token: thisIsMyToken
            name: Test Power Outlet
            device: Test Device
            state: present

        - name: Update power port with other fields
          networktocode.nautobot.power_outlet:
            url: http://nautobot.local
            token: thisIsMyToken
            name: Test Power Outlet
            device: Test Device
            type: iec-60320-c6
            power_port: Test Power Port
            feed_leg: A
            description: power port description
            state: present

        - name: Delete power port within nautobot
          networktocode.nautobot.power_outlet:
            url: http://nautobot.local
            token: thisIsMyToken
            name: Test Power Outlet
            device: Test Device
            state: absent




.. Facts


.. Return values

Return Values
-------------
Common return values are documented :ref:`here <common_return_values>`, the following are the fields unique to this module:

.. raw:: html

    <table border=0 cellpadding=0 class="documentation-table">
        <tr>
            <th colspan="1">Key</th>
            <th>Returned</th>
            <th width="100%">Description</th>
        </tr>
                    <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-msg"></div>
                    <b>msg</b>
                    <a class="ansibleOptionLink" href="#return-msg" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">string</span>
                                          </div>
                                    </td>
                <td>always</td>
                <td>
                                            <div>Message indicating failure or info about what has been achieved</div>
                                        <br/>
                                    </td>
            </tr>
                                <tr>
                                <td colspan="1">
                    <div class="ansibleOptionAnchor" id="return-power_outlet"></div>
                    <b>power_outlet</b>
                    <a class="ansibleOptionLink" href="#return-power_outlet" title="Permalink to this return value"></a>
                    <div style="font-size: small">
                      <span style="color: purple">dictionary</span>
                                          </div>
                                    </td>
                <td>success (when <em>state=present</em>)</td>
                <td>
                                            <div>Serialized object as created or already existent within Nautobot</div>
                                        <br/>
                                    </td>
            </tr>
                        </table>
    <br/><br/>

..  Status (Presently only deprecated)


.. Authors

Authors
~~~~~~~

- Tobias Groß (@toerb)



.. Parsing errors

